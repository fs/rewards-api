# User Profiles API

## List of bonus possibilities for current user

### GET /api/v1/user/profile
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1ODA4OTE1MjcsInN1YiI6NDYxLCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.Txf-ZYuBgzmtVxS6SN9RD-QcTvq_uOqnM3rByUSZhz0</pre>

#### Route

<pre>GET /api/v1/user/profile</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.flts.tk/api/v1/user/profile&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1ODA4OTE1MjcsInN1YiI6NDYxLCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.Txf-ZYuBgzmtVxS6SN9RD-QcTvq_uOqnM3rByUSZhz0&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": {
    "id": "461",
    "type": "users",
    "attributes": {
      "email": "analisa_friesen@runolfsdottirwest.co",
      "full-name": "Aldo Lubowitz",
      "username": "lubowitz.aldo",
      "profile-image-avatar-url": "memory://user/profile_image/a4c5ec27c1060f63a4d4ca0ceb68d909.png",
      "bonus-balance": 10000,
      "allowance-balance": 10000,
      "birth-date": "2001-09-24"
    }
  }
}</pre>
