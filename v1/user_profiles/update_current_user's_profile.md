# User Profiles API

## Update current user&#39;s profile

### PATCH /api/v1/user/profile

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| full_name | Full Name | false |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzAsInN1YiI6MzIyMSwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.fdiFFuk4lcbMjd9-82x-uOcgqZYCZDmrfOcM7MlVz9Q</pre>

#### Route

<pre>PATCH /api/v1/user/profile</pre>

#### Body

<pre>{"data":{"id":"updateprofilerequest","type":"update-profile-requests","attributes":{"full-name":"New Full Name"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/user/profile&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;updateprofilerequest&quot;,&quot;type&quot;:&quot;update-profile-requests&quot;,&quot;attributes&quot;:{&quot;full-name&quot;:&quot;New Full Name&quot;}}}&#39; -X PATCH \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzAsInN1YiI6MzIyMSwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.fdiFFuk4lcbMjd9-82x-uOcgqZYCZDmrfOcM7MlVz9Q&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": {
    "id": "3221",
    "type": "users",
    "attributes": {
      "email": "hong@mrazjakubowski.com",
      "full-name": "New Full Name",
      "username": "orn-marta",
      "profile-image-avatar-url": "memory://user/profile_image/81311571b74e4c8da9fe67dbea58b386.png",
      "bonus-balance": 10000,
      "allowance-balance": 10000,
      "birth-date": "1971-01-05"
    }
  }
}</pre>
