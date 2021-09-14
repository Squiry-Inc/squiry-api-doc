# Add Payment

{% api-method method="post" host="https://api.payant.ng/payments" path="" %}
{% api-method-summary %}
Add Payment
{% endapi-method-summary %}

{% api-method-description %}
The Add Payment endpoint allows you to add a manual payment to Payant.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Your Payant Secret Key.  prefixed with "Bearer "
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="reference\_code" type="string" required=true %}
Invoice reference code
{% endapi-method-parameter %}

{% api-method-parameter name="amount" type="string" required=true %}
Payment amount
{% endapi-method-parameter %}

{% api-method-parameter name="channel" type="string" required=true %}
Payment channel `Cash`, `BankTransfer`, `POS` or `Cheque`
{% endapi-method-parameter %}

{% api-method-parameter name="notes" type="string" required=false %}
Brief notes on Payment
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
  "message": "Payment successful.",
  "data": {
    "company_id": "1",
    "client_id": "1",
    "invoice_id": "1",
    "expense_id": "",
    "amount": "50000.00",
    "currency": "NGN",
    "transaction_date": "1482105600",
    "status": "success",
    "reference_code": "j9CbiTN0oJe4vWhglyS2",
    "payment_id": "",
    "referrer": "",
    "gateway_response": "",
    "message": "",
    "channel": "Cash",
    "type": "Invoice",
    "created_at": "2016-12-21 18:46:30",
    "updated_at": "2016-12-21 18:46:30",
    "id": 1,
    "client": {
        "id": 1
        "company_id": 1,
        "name": "Albert Specialist Hospital",
        "first_name": "Albert",
        "last_name": "Jane",
        "email": "jane@alberthospital.com",
        "phone": "+2348012345678",
        "website": "http://www.alberthospital.com",
        "address": "Wase II",
        "type": "Customer",
        "settlement_bank": "",
        "account_name": "",
        "account_number": "",
        "status": "1",
        "created_at": "2016-12-21 17:19:10",
        "updated_at": "2016-12-21 17:19:10",
        "deleted_at": null
    },
    invoice: {
        "id": 1,
        "company_id": "1",
        "client_id": "1",
        "reference_code": "j9CbiTN0oJe4vWhglyS2",
        "payment_id": null,
        "fee_bearer": "client",
        "mail_status": "unsent",
        "status": "0",
        "due_date": "1483056000",
        "created_at": "2016-12-21 18:46:30",
        "updated_at": "2016-12-21 18:46:30",
        "deleted_at": null,
        "items": [
            {
                "id": "1",
                "company_id": "1",
                "client_id": "1",
                "name": "Website Design",
                "description": "5 Pages Website plus 1 Year Web Hosting",
                "quantity": "1",
                "unit_cost": "50000.00",
                "status": "0",
                "due_date": "1483056000",
                "created_at": "2016-12-21 17:19:10",
                "updated_at": "2016-12-21 17:19:10",
                "deleted_at": null
            }
        ]
    }
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.payant.ng/payments/:reference\_code" path="" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}

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

{% api-method method="get" host="https://api.payant.ng/payments/:reference\_code" path="" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}

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

### Request

```bash
curl https://api.payant.ng/payments \
-H "Content-Type: application/json" \
-H "Authorization: Bearer SECRET_KEY" \
-d '{ "reference_code": "j9CbiTN0oJe4vWhglyS2",
        "amount": "50,000.00",
        "channel": "Cash" }' \
-X POST 
```

### Response

```javascript
{
  "status": "success",
  "message": "Payment successful.",
  "data": {
    "company_id": "1",
    "client_id": "1",
    "invoice_id": "1",
    "expense_id": "",
    "amount": "50000.00",
    "currency": "NGN",
    "transaction_date": "1482105600",
    "status": "success",
    "reference_code": "j9CbiTN0oJe4vWhglyS2",
    "payment_id": "",
    "referrer": "",
    "gateway_response": "",
    "message": "",
    "channel": "Cash",
    "type": "Invoice",
    "created_at": "2016-12-21 18:46:30",
    "updated_at": "2016-12-21 18:46:30",
    "id": 1,
    "client": {
        "id": 1
        "company_id": 1,
        "name": "Albert Specialist Hospital",
        "first_name": "Albert",
        "last_name": "Jane",
        "email": "jane@alberthospital.com",
        "phone": "+2348012345678",
        "website": "http://www.alberthospital.com",
        "address": "Wase II",
        "type": "Customer",
        "settlement_bank": "",
        "account_name": "",
        "account_number": "",
        "status": "1",
        "created_at": "2016-12-21 17:19:10",
        "updated_at": "2016-12-21 17:19:10",
        "deleted_at": null
    },
    invoice: {
        "id": 1,
        "company_id": "1",
        "client_id": "1",
        "reference_code": "j9CbiTN0oJe4vWhglyS2",
        "payment_id": null,
        "fee_bearer": "client",
        "mail_status": "unsent",
        "status": "0",
        "due_date": "1483056000",
        "created_at": "2016-12-21 18:46:30",
        "updated_at": "2016-12-21 18:46:30",
        "deleted_at": null,
        "items": [
            {
                "id": "1",
                "company_id": "1",
                "client_id": "1",
                "name": "Website Design",
                "description": "5 Pages Website plus 1 Year Web Hosting",
                "quantity": "1",
                "unit_cost": "50000.00",
                "status": "0",
                "due_date": "1483056000",
                "created_at": "2016-12-21 17:19:10",
                "updated_at": "2016-12-21 17:19:10",
                "deleted_at": null
            }
        ]
    }
  }
}
```

