# Check Enrollment Status

{% api-method method="get" host="https://us-central1-squiry-4f678.cloudfunctions.net/api/check-enrollment/:courseId" path="" %}
{% api-method-summary %}
Check User Enrollment status for a Course
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
Id token prefixed by "Bearer "
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```

{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

### **Request**

```bash
curl https://us-central1-squiry-4f678.cloudfunctions.net/api/check-enrollment/AwWaRuYt94iCex4rtE4X \
-H "Content-Type: application/json" \
-H "Authorization: Bearer ID_TOKEN" \
-X GET
```

### **Response**

```javascript
{
   "status": true,
   "message": "User Already Enrolled"
}

or

{
   "status": false,
   "message": "Not Enrolled"
}
```
