# Getting All Courses

{% api-method method="get" host="https://us-central1-squiry-4f678.cloudfunctions.net/api/courses-all" path="" %}
{% api-method-summary %}
Get all Currently published Courses
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="No headers" type="" required=false %}

{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="No body" type="string" required=false %}
NO body
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "status": "success",
  "data": {
    "courses": [
        {
            "course_id": "j9CbiTN0oJe4vWhglyS2",
            "course_title": "Shopify dropshipping",
            "thumbnail": "https://via.placeholder.com/150",
            "author": "sample",
            "course_desc": "lorem ipsum dolor sit amet, consectetur adipiscing elit...",
            "created_at": "2016-12-21 18:46:30",
            "course_topics": ["j9CbiTN0oJe4vWhg","j9CbiTN0oJe4vWhg","j9CbiTN0oJe4vWhg"],
            "published": true,
            "video_preview": "https://www.vimeo.com/vidoe/why-shopify",
        },
        {
            "course_id": "j9CbiTN0oJe4vWhglyS2",
            "course_title": "Shopify dropshipping",
            "thumbnail": "https://via.placeholder.com/150",
            "author": "sample",
            "course_desc": "lorem ipsum dolor sit amet, consectetur adipiscing elit...",
            "created_at": "2016-12-21 18:46:30",
            "course_topics": ["j9CbiTN0oJe4vWhg","j9CbiTN0oJe4vWhg","j9CbiTN0oJe4vWhg"],
            "published": true,
            "video_preview": "https://www.vimeo.com/vidoe/why-shopify",
        },
    ]
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

## Request

```bash
curl https://api.payant.ng/invoices \
-H "Content-Type: application/json" \
-X GET
```

## Response

```javascript
{
  "status": "success",
  "data": {
    "courses": [
        {
            "course_id": "j9CbiTN0oJe4vWhglyS2",
            "course_title": "Shopify dropshipping",
            "thumbnail": "https://via.placeholder.com/150",
            "author": "sample",
            "course_desc": "lorem ipsum dolor sit amet, consectetur adipiscing elit...",
            "created_at": "2016-12-21 18:46:30",
            "course_topics": ["j9CbiTN0oJe4vWhg","j9CbiTN0oJe4vWhg","j9CbiTN0oJe4vWhg"],
            "published": true,
        },
        {
            "course_id": "j9CbiTN0oJe4vWhglyS2",
            "course_title": "Shopify dropshipping",
            "thumbnail": "https://via.placeholder.com/150",
            "author": "sample",
            "course_desc": "lorem ipsum dolor sit amet, consectetur adipiscing elit...",
            "created_at": "2016-12-21 18:46:30",
            "course_topics": ["j9CbiTN0oJe4vWhg","j9CbiTN0oJe4vWhg","j9CbiTN0oJe4vWhg"],
            "published": true,
        },
    ]
  }
}
```

