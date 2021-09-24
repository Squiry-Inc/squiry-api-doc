# Getting A Course

{% api-method method="get" host="https://us-central1-squiry-4f678.cloudfunctions.net/api/topic/:topicId" path="" %}
{% api-method-summary %}
Get a course
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

```text

```

{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

## **Request**

```bash
curl https://us-central1-squiry-4f678.cloudfunctions.net/api/course/AwWaRuYt94iCex4rtE4X \
-H "Content-Type: application/json" \
-H "Authorization: Bearer ID_TOKEN" \
-X GET
```

## **Response**

```javascript
{
   "course_id": "1cCWUY8K1Fk5VvMtHupn",
   "title": "Dropshipping Masterclass",
   "description": "lorem ipsum dolor sit amet, consectet...",
   "author": "sample",
   "thumbnail": "https://via.placeholder.com/150",
   "created_at": "2016-12-21 18:46:30",
   "published": true,
   "video_preview": "https://www.vimeo.com/vidoe/why-shopify",
   "course_topics": [
      {
      "id": "NFZoOu5mCxWdgRcz3hMk",
      "title": "Addition of Numbers"
      }
   ]
}
```
