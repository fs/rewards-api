# Bot Users API

## List users

### GET /api/v1/bot/users
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzQsInN1YiI6MTd9.DxGf19jetk7BBHuxxYZmK-QYnGCsdd-zvVZXxkVBUOY</pre>

#### Route

<pre>GET /api/v1/bot/users</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.flts.tk/api/v1/bot/users&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzQsInN1YiI6MTd9.DxGf19jetk7BBHuxxYZmK-QYnGCsdd-zvVZXxkVBUOY&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{"data":[{"id":"291","type":"users","attributes":{"email":"lucie.doyle@flatstack.com","full-name":"Elian Windler IV","username":"elian-iv-windler","profile-image-avatar-url":"memory://user/profile_image/12cad387737728ce76d36c7434fb6c37.png","allowance-balance":10000}}]}</pre>
