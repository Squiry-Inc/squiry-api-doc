# Authentication

Squiry API uses id tokens to authenticate requests. You can get an id token when ever a user is logged in to the application.

All requests to the Squiry API must be authenticated by including the `id token` in request headers.

Your authorization header should be like:`Authorization: Bearer cd525b1d647942a21c51d03f8c07e2fd43b4e955ec13a8c54c8a5f2d`

All API requests must be made over [HTTPS](http://en.wikipedia.org/wiki/HTTP_Secure). Calls made over plain HTTP will fail. API requests without authentication will also fail.

{% page-ref page="test-cards-and-bank-accounts.md" %}

{% hint style="info" %}
**Heads up!**

Your id token carry many privileges, so be sure to keep them secure! Do not share your Private API keys in publicly accessible areas such as GitHub, client-side code, and so forth.
{% endhint %}
