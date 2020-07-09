# User Profiles API

## List of bonus possibilities for current user

### GET /api/v1/user/profile
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzEsInN1YiI6MzIyMywidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.XrYfo4qr6N2zS5LX1QU7aaaFStzdzdPLMaZuMGIw3YA</pre>

#### Route

<pre>GET /api/v1/user/profile</pre>

#### Query Parameters

<pre>{}: </pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/profile&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzEsInN1YiI6MzIyMywidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.XrYfo4qr6N2zS5LX1QU7aaaFStzdzdPLMaZuMGIw3YA&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": {
    "id": "3223",
    "type": "users",
    "attributes": {
      "email": "ahmed@marks.info",
      "full-name": "Neomi Koss",
      "username": "koss.neomi",
      "profile-image-avatar-url": "memory://user/profile_image/e313cb242e8935d011062e115e37ebb3.png",
      "bonus-balance": 10000,
      "allowance-balance": 10000,
      "birth-date": "1973-02-09"
    }
  }
}</pre>
