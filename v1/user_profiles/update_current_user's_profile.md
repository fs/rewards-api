# User Profiles API

## Update current user&#39;s profile

### PATCH /api/v1/user/profile

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| full_name | Full Name | false |  |
| username | Username | false |  |
| email_notification | Email Notifications Enabled | false |  |
| email | Email | false |  |
| password | New password | false |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzIsInN1YiI6MTk1NCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.zgrKQvgf94xOz7iu5RHYXL45NEl7_lAa019ysbSZNNA</pre>

#### Route

<pre>PATCH /api/v1/user/profile</pre>

#### Body

<pre>{"data":{"id":"updateprofilerequest","type":"update-profile-requests","attributes":{"full-name":"New Full Name","username":"NewUsername","email":"test@test.com","email-notification":false,"password":"qwerty123"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/user/profile&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;updateprofilerequest&quot;,&quot;type&quot;:&quot;update-profile-requests&quot;,&quot;attributes&quot;:{&quot;full-name&quot;:&quot;New Full Name&quot;,&quot;username&quot;:&quot;NewUsername&quot;,&quot;email&quot;:&quot;test@test.com&quot;,&quot;email-notification&quot;:false,&quot;password&quot;:&quot;qwerty123&quot;}}}&#39; -X PATCH \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzIsInN1YiI6MTk1NCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.zgrKQvgf94xOz7iu5RHYXL45NEl7_lAa019ysbSZNNA&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": {
    "id": "1954",
    "type": "users",
    "attributes": {
      "email": "test@test.com",
      "full-name": "Ms. Rossana Schaden",
      "username": "NewUsername",
      "profile-image-avatar-url": "memory://user/profile_image/1dc8cdd503c6b3249a65f2bf71f9e4e6.png",
      "bonus-balance": 10000,
      "allowance-balance": 10000,
      "birth-date": "1986-07-18"
    }
  }
}</pre>
