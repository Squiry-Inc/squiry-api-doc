# Enrolling in A Course

{% api-method method="post" host="https://us-central1-squiry-4f678.cloudfunctions.net/api/enroll/:courseId" path="" %}
{% api-method-summary %}
Enroll A User into A Course
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="courseId" type="string" required=true %}
Course Id
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
id token prefixed by "Bearer "
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=201 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```text

```

{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

## **Request**

```bash
curl https://us-central1-squiry-4f678.cloudfunctions.net/api/enroll/fIWTG1Z5S79ncTHMRUPl \
-H "Content-Type: application/json" \
-H "Authorization: Bearer ID_TOKEN" \
-X POST
```

## **Response**

```javascript
{
  "status": "success",
  "message": "Congratulations you have been successfully enrolled"
}
```
