# Bot Users API

## List users

### GET /api/v1/bot/users
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzEsInN1YiI6OTIsInR5cGUiOiJhY2Nlc3MiLCJjbGllbnRfaWQiOiIyIn0.iMKGgnRuPne_x12Uglu2sYrN9bKX0CcipmJ4E_XvEtA</pre>

#### Route

<pre>GET /api/v1/bot/users</pre>

#### Query Parameters

<pre>{}: </pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/bot/users&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzEsInN1YiI6OTIsInR5cGUiOiJhY2Nlc3MiLCJjbGllbnRfaWQiOiIyIn0.iMKGgnRuPne_x12Uglu2sYrN9bKX0CcipmJ4E_XvEtA&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": [
    {
      "id": "3226",
      "type": "users",
      "attributes": {
        "email": "earl_ruecker@hudson.com",
        "full-name": "Enda Jacobi",
        "username": "enda.jacobi",
        "profile-image-avatar-url": "memory://user/profile_image/2e301a4fd44ab2ce5c3de29b764a68c5.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "2006-05-01"
      }
    }
  ]
}</pre>
