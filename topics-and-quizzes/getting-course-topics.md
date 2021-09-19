# Getting Course Topics

{% api-method method="get" host="https://us-central1-squiry-4f678.cloudfunctions.net/api/:courseId/topics" path="" %}
{% api-method-summary %}
Getting topics in a course
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="courseId" type="string" required=true %}
courseId
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Id token prefixed with bearer
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
curl https://us-central1-squiry-4f678.cloudfunctions.net/api/user-courses \
-H "Content-Type: application/json" \
-H "Authorization: Bearer ID_TOKEN" \
-X GET
```

## **Response**

```javascript
{
  "topics": [
       {
            "topic_id": "1cCWUY8K1Fk5VvMtHupn",
            "author": "sample",
            "title": "Why dropship on Shopify",
            "description": "lorem ipsum dolor sit amet, consectet...",
            "video_url": "https://www.vimeo.com/vidoe/why-shopify",
            "material": "https://www.squiry.com/file/shopify.pdf",
            "course_id": "j9CbiTN0oJe4vWhglyS2"
        },
        {
            "topic_id": "1cCWUY8K1Fk5VvMtHupn",
            "author": "sample",
            "title": "Why dropship on Shopify",
            "description": "lorem ipsum dolor sit amet, consectet...",
            "video_url": "https://www.vimeo.com/vidoe/why-shopify",
            "material": "https://www.squiry.com/file/shopify.pdf",
            "course_id": "j9CbiTN0oJe4vWhglyS2"
        },
    ]
}
```

