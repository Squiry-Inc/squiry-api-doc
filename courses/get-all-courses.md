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
        "course_id": "jhNdzdNUAqxSAAAR5opl",
        "course_title": "Use of English",
        "description": "English language, West Germanic language of the Indo-European language family that is closely related to the Frisian, German, and Dutch (in Belgium called Flemish) languages. English originated in England and is the dominant language of the United States, the United Kingdom, Canada, Australia, Ireland, New Zealand, and various island nations in the Caribbean Sea and the Pacific Ocean.",
        "published": true,
        "author": "sample",
        "thumbnail": "https://firebasestorage.googleapis.com/v0/b/squiry-4f678.appspot.com/o/english.png?alt=media",
        "created_at": "2021-09-05T18:51:27.958Z",
        "video_preview": "https://www.youtube.com/watch?v=u-JpkH2RCns"
      },
      {
        "course_id": "bcWQnq4e7vTWokUYzD3W",
        "course_title": "Basic Mathematics",
        "description": "Basic math? Simply put, you use basic mathematics almost every day of your life. You use it at home, on the job, or when you go to school. See what basic math looks like with our representation below.\nAt home, you may for instance have a budget to help manage your income and probably put some money aside. If your monthly income is 1000 dollars, 50% may go to your rent or mortgage;\n\n20% may go to food, clothing, gas, and other utilities; 20% may be used for personal items, gift",
        "published": true,
        "author": "sample",
        "thumbnail": "https://firebasestorage.googleapis.com/v0/b/squiry-4f678.appspot.com/o/mathematics.png?alt=media",
        "created_at": "2021-09-08T07:36:19.464Z",
        "course_topics": [
          {
            "id": "NFZoOu5mCxWdgRcz3hMk",
            "title": "Addition of Numbers"
          }
        ],
        "video_preview": "https://www.youtube.com/watch?v=T_6Mq6PWoGc"
      },
      {
        "course_id": "jvgGlMNLJMaxLF8O4K9f",
        "course_title": "Shopfiy Drop shipping Masterclass",
        "description": "The Complete Shopify Dropshipping Masterclass 2.0 Is Aimed For Complete Beginners & Can Also Help More Experienced Shopify Dropshipping Owners. In this Course, We'll Take You From Being an Absolute Beginner to Have a Shopify Dropshipping Business Up and Running Within Hours!",
        "published": true,
        "author": "sample",
        "thumbnail": "https://firebasestorage.googleapis.com/v0/b/squiry-4f678.appspot.com/o/Shopify.jpg?alt=media",
        "created_at": "2021-08-26T07:46:31.044Z",
        "course_topics": [
          "ExKwr28lVrNCdaVgKksU",
          "1cCWUY8K1Fk5VvMtHupn"
        ],
        "video_preview": "https://youtu.be/jXIPUqrKyjI"
      }
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
curl https://us-central1-squiry-4f678.cloudfunctions.net/api/courses-all \
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
        "course_id": "bcWQnq4e7vTWokUYzD3W",
        "course_title": "Basic Mathematics",
        "thumbnail": "https://firebasestorage.googleapis.com/v0/b/squiry-4f678.appspot.com/o/mathematics.png?alt=media",
        "author": "sample",
        "course_desc": "Basic math? Simply put, you use basic mathematics almost every day of your life. You use it at home, on the job, or when you go to school. See what basic math looks like with our representation below.\nAt home, you may for instance have a budget to help manage your income and probably put some money aside. If your monthly income is 1000 dollars, 50% may go to your rent or mortgage;\n\n20% may go to food, clothing, gas, and other utilities; 20% may be used for personal items, gift",
        "created_at": "2021-09-08T07:36:19.464Z",
        "course_topics": [
          {
            "id": "NFZoOu5mCxWdgRcz3hMk",
            "title": "Addition of Numbers"
          }
        ],
        "published": true,
        "video_preview": "https://www.youtube.com/watch?v=T_6Mq6PWoGc"
      },
      {
        "course_id": "jhNdzdNUAqxSAAAR5opl",
        "course_title": "Use of English",
        "thumbnail": "https://firebasestorage.googleapis.com/v0/b/squiry-4f678.appspot.com/o/english.png?alt=media",
        "author": "sample",
        "course_desc": "English language, West Germanic language of the Indo-European language family that is closely related to the Frisian, German, and Dutch (in Belgium called Flemish) languages. English originated in England and is the dominant language of the United States, the United Kingdom, Canada, Australia, Ireland, New Zealand, and various island nations in the Caribbean Sea and the Pacific Ocean.",
        "created_at": "2021-09-05T18:51:27.958Z",
        "published": true,
        "video_preview": "https://www.youtube.com/watch?v=u-JpkH2RCns"
      },
      {
        "course_id": "jvgGlMNLJMaxLF8O4K9f",
        "course_title": "Shopfiy Drop shipping Masterclass",
        "thumbnail": "https://firebasestorage.googleapis.com/v0/b/squiry-4f678.appspot.com/o/Shopify.jpg?alt=media",
        "author": "sample",
        "course_desc": "The Complete Shopify Dropshipping Masterclass 2.0 Is Aimed For Complete Beginners & Can Also Help More Experienced Shopify Dropshipping Owners. In this Course, We'll Take You From Being an Absolute Beginner to Have a Shopify Dropshipping Business Up and Running Within Hours!",
        "created_at": "2021-08-26T07:46:31.044Z",
        "course_topics": [
          "ExKwr28lVrNCdaVgKksU",
          "1cCWUY8K1Fk5VvMtHupn"
        ],
        "published": true,
        "video_preview": "https://youtu.be/jXIPUqrKyjI"
      }
    ]
  }
}
```
