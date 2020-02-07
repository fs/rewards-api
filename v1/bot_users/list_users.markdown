# Bot Users API

## List users

### GET /api/v1/bot/users
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1ODA4OTE1MjMsInN1YiI6MjEsInR5cGUiOiJhY2Nlc3MiLCJjbGllbnRfaWQiOiIyIn0.4HkInMn_fsoTO193ZalaRmsxilISut-rJ_D4TlTCrE0</pre>

#### Route

<pre>GET /api/v1/bot/users</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.flts.tk/api/v1/bot/users&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1ODA4OTE1MjMsInN1YiI6MjEsInR5cGUiOiJhY2Nlc3MiLCJjbGllbnRfaWQiOiIyIn0.4HkInMn_fsoTO193ZalaRmsxilISut-rJ_D4TlTCrE0&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": [
    {
      "id": "421",
      "type": "users",
      "attributes": {
        "email": "emmitt_marks@waterswaelchi.io",
        "full-name": "Cherie Simonis",
        "username": "cherie_simonis",
        "profile-image-avatar-url": "memory://user/profile_image/702430f53169f996ffa0c8ccdfae15e0.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "1979-10-23"
      }
    }
  ]
}</pre>
