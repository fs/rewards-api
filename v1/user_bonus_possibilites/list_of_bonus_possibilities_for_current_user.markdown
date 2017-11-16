# User Bonus Possibilites API

## List of bonus possibilities for current user

### GET /api/v1/user/bonus_possibilities
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzQsInN1YiI6Mjg3fQ.H-noT6eMnVKMTubCnSV42urygeBDv3dG2j6Liy-kzXI</pre>

#### Route

<pre>GET /api/v1/user/bonus_possibilities</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.flts.tk/api/v1/user/bonus_possibilities&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzQsInN1YiI6Mjg3fQ.H-noT6eMnVKMTubCnSV42urygeBDv3dG2j6Liy-kzXI&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{"data":{"id":"287","type":"bonus-possibilities","relationships":{"amounts":{"data":[{"id":"50","type":"points"},{"id":"250","type":"points"},{"id":"500","type":"points"},{"id":"750","type":"points"},{"id":"1000","type":"points"},{"id":"1250","type":"points"}]},"tags":{"data":[{"id":"393","type":"tags"}]},"receivers":{"data":[{"id":"286","type":"users"}]}}},"included":[{"id":"50","type":"points","attributes":{"value":50}},{"id":"250","type":"points","attributes":{"value":250}},{"id":"500","type":"points","attributes":{"value":500}},{"id":"750","type":"points","attributes":{"value":750}},{"id":"1000","type":"points","attributes":{"value":1000}},{"id":"1250","type":"points","attributes":{"value":1250}},{"id":"393","type":"tags","attributes":{"label":"laboriosam-aut-qui"}},{"id":"286","type":"users","attributes":{"email":"shane.osinski@flatstack.com","full-name":"Alta Grady","username":"grady_alta","profile-image-avatar-url":"memory://user/profile_image/f0652bd66f657a89ad0e8565382c86d8.png","allowance-balance":10000}}]}</pre>
