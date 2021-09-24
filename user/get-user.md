# Get User

{% api-method method="get" host="https://us-central1-squiry-4f678.cloudfunctions.net/api/user" path="" %}
{% api-method-summary %}
Getting a user data
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
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

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

## **Request**

```bash
curl https://us-central1-squiry-4f678.cloudfunctions.net/api//user \
-H "Content-Type: application/json" \
-H "Authorization: Bearer ID_TOKEN" \
-X GET
```

## **Response**

```javascript
{
  "user_id": "1cCWUY8K1Fk5VvMtHupn",
  "username": "sample",
  "full_name": "Sample User",
  "email": "example@email.com",
  "phone_number": "08123456789",
  "role": "student",
  "about_me": "lorem ipsum dolor sit amet, consectet...",
  "image_url": "https://www.squiry.com/avatar/sample.png",
  "institution": "Bayero University Kano - BUK",
  "state": "Lagos, Nigeria",
  "enrolled_courses": ["j9CbiTN0oJe4vWhglyS2", "j9CbiTN0oJe4vWhglyS2"],
  "created_at": "2021-8-10T10:18:53.500Z"
  "updated_at": "2021-8-10T10:18:53.500Z"
}
```

