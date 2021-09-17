# Get User Courses

{% api-method method="get" host="https://us-central1-squiry-4f678.cloudfunctions.net/api/user-courses" path="" %}
{% api-method-summary %}
Getting User Enrolled Courses
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
id token prefixed with "Bearer "
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
curl https://us-central1-squiry-4f678.cloudfunctions.net/api/user-courses \
-H "Content-Type: application/json" \
-H "Authorization: Bearer ID_TOKEN" \
-X GET
```

### **Response**

```javascript
{
  "status": "success",
  "data": {
    "courses": [
        {
            "course_id": "j9CbiTN0oJe4vWhglyS2",
            "course_title": "Shopify dropshipping",
            "description": "lorem ipsum dolor sit amet, consectetur adipiscing elit...",
            "published": true,
            "author": "sample",
            "thumbnail": "https://via.placeholder.com/150",
            "created_at": "2016-12-21 18:46:30",
            "course_topics": ["j9CbiTN0oJe4vWhg","j9CbiTN0oJe4vWhg","j9CbiTN0oJe4vWhg"]
        },
        {
            "course_id": "j9CbiTN0oJe4vWhglyS2",
            "course_title": "Shopify dropshipping",
            "description": "lorem ipsum dolor sit amet, consectetur adipiscing elit...",
            "published": true,
            "author": "sample",
            "thumbnail": "https://via.placeholder.com/150",
            "created_at": "2016-12-21 18:46:30",
            "course_topics": ["j9CbiTN0oJe4vWhg","j9CbiTN0oJe4vWhg","j9CbiTN0oJe4vWhg"]
        }
    ]
  }
}
```
