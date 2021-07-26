# User Profiles API

## List of bonus possibilities for current user

### GET /api/v1/user/profile
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzIsInN1YiI6MTk1MSwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.p2WDFpohjo0PGEpw1ZsU1mNL-IlaBua8O9IAWtnGeSE</pre>

#### Route

<pre>GET /api/v1/user/profile</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/profile&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzIsInN1YiI6MTk1MSwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.p2WDFpohjo0PGEpw1ZsU1mNL-IlaBua8O9IAWtnGeSE&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": {
    "id": "1951",
    "type": "users",
    "attributes": {
      "email": "jason.marks@ryan.com",
      "full-name": "Jewel Blanda",
      "username": "jewel-blanda",
      "profile-image-avatar-url": "memory://user/profile_image/33e1c2a369351d607cc00936fbb8ebef.png",
      "bonus-balance": 10000,
      "allowance-balance": 10000,
      "birth-date": "1980-05-29"
    }
  }
}</pre>
