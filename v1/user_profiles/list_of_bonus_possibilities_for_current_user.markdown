# User Profiles API

## List of bonus possibilities for current user

### GET /api/v1/user/profile
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzUsInN1YiI6Mjk2fQ.0a2jfk8gWEJsBVnDcjyL4AOiIp6QQW13_tyJivM2fAk</pre>

#### Route

<pre>GET /api/v1/user/profile</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.flts.tk/api/v1/user/profile&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzUsInN1YiI6Mjk2fQ.0a2jfk8gWEJsBVnDcjyL4AOiIp6QQW13_tyJivM2fAk&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{"data":{"id":"296","type":"users","attributes":{"email":"jayne.torphy@flatstack.com","full-name":"Cory Stiedemann","username":"stiedemann-cory","profile-image-avatar-url":"memory://user/profile_image/93e3cf35bbcb33cc2299ff5aab91cf97.png","allowance-balance":10000}}}</pre>
