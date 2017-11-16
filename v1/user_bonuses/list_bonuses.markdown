# User Bonuses API

## List bonuses

### GET /api/v1/user/bonuses
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzMsInN1YiI6Mjc0fQ.E9QHRo7JSOSJxohX01VtQr7g7YYrP4pTa3GcDPPG2x8</pre>

#### Route

<pre>GET /api/v1/user/bonuses</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.flts.tk/api/v1/user/bonuses&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzMsInN1YiI6Mjc0fQ.E9QHRo7JSOSJxohX01VtQr7g7YYrP4pTa3GcDPPG2x8&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{"data":[{"id":"44","type":"bonuses","attributes":{"text":"+31 to @phd.dortha.bruen #facere-alias-qui Thank you!","points":31,"total-points":43,"created-at":"2017-11-16T12:31:13.459Z"},"relationships":{"sender":{"data":{"id":"272","type":"users"}},"comments":{"data":[]}}},{"id":"43","type":"bonuses","attributes":{"text":"+16 to @homenick.mr.terrell #dolores-ipsa-aperiam Thank you!","points":16,"total-points":85,"created-at":"2017-11-16T12:31:13.408Z"},"relationships":{"sender":{"data":{"id":"270","type":"users"}},"comments":{"data":[]}}}],"included":[{"id":"272","type":"users","attributes":{"full-name":"Constantin Pacocha"}},{"id":"270","type":"users","attributes":{"full-name":"Malcolm Ankunding III"}}],"links":{"self":"http://example.org/api/v1/user/bonuses?page%5Bnumber%5D=1\u0026page%5Bsize%5D=10","first":"http://example.org/api/v1/user/bonuses?page%5Bnumber%5D=1\u0026page%5Bsize%5D=10","prev":null,"next":null,"last":"http://example.org/api/v1/user/bonuses?page%5Bnumber%5D=1\u0026page%5Bsize%5D=10"}}</pre>
