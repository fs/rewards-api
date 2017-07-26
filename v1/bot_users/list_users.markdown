# Bot Users API

## List users

### GET /api/v1/bot/users
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MDExNTIxNTEsInN1YiI6OTN9.PNhBiABmNRY-qHl5o7lIKTR0qfGvON-L0yQc_wHHhoU</pre>

#### Route

<pre>GET /api/v1/bot/users</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.flts.tk/api/v1/bot/users&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MDExNTIxNTEsInN1YiI6OTN9.PNhBiABmNRY-qHl5o7lIKTR0qfGvON-L0yQc_wHHhoU&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{"data":[{"id":"496","type":"users","attributes":{"email":"denis@flatstack.com","full-name":"Frederique Dibbert","username":"dibbert.frederique","profile-image-avatar-url":"memory://user/profile_image/d976720f7415d1f2815599e8673defcd.png"}}]}</pre>
