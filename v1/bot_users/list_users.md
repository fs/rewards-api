# Bot Users API

## List users

### GET /api/v1/bot/users
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzMsInN1YiI6NjEsInR5cGUiOiJhY2Nlc3MiLCJjbGllbnRfaWQiOiIyIn0.EWRs_jXZLAZqbNsAj7smCq5rub4B0xNCGMyrkeKWbL8</pre>

#### Route

<pre>GET /api/v1/bot/users</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/bot/users&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzMsInN1YiI6NjEsInR5cGUiOiJhY2Nlc3MiLCJjbGllbnRfaWQiOiIyIn0.EWRs_jXZLAZqbNsAj7smCq5rub4B0xNCGMyrkeKWbL8&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": [
    {
      "id": "1955",
      "type": "users",
      "attributes": {
        "email": "dinorah_klein@bartoletti.io",
        "full-name": "Velva Huel MD",
        "username": "md_velva_huel",
        "profile-image-avatar-url": "memory://user/profile_image/41b565b4ad43448ac4420f94942de79b.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "1995-08-01"
      }
    }
  ]
}</pre>
