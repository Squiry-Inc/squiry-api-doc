# Get Institutions

{% api-method method="get" host="https://us-central1-squiry-4f678.cloudfunctions.net/api/institutions" path="" %}
{% api-method-summary %}
Get List of Institutions
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="" required=false %}
No Params
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

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
curl https://us-central1-squiry-4f678.cloudfunctions.net/api/institutions \
-H "Content-Type: application/json" \
-X GET
```

### **Response**

```javascript
{
  "status": "success",
  "data": [
    {
      "institutionName": "Bayero University Kano",
      "institutionAbbr": "BUK",
      "institutionLocation": "Kano, Kano, Nigeria",
    },
    {
      "institutionName": "Ahmadu Bello University",
      "institutionAbbr": "ABU",
      "institutionLocation": "Zaria, Kaduna, Nigeria",
    },
    {
      "institutionName": "University of Maiduguri",
      "institutionAbbr": "UNIMAID",
      "institutionLocation": "Maiduguri, Borno, Nigeria",
    },
  ],

}
```
