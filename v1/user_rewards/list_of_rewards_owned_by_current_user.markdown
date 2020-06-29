# User Rewards API

## List of rewards owned by current user

### GET /api/v1/user/rewards
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTM1MTE1NzEsInN1YiI6Mzc3LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.B9_Z9X_TfW6sn1meGvO3ZrVD4TjSCsPyzzW-JPAcdP4</pre>

#### Route

<pre>GET /api/v1/user/rewards</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.flts.tk/api/v1/user/rewards&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTM1MTE1NzEsInN1YiI6Mzc3LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.B9_Z9X_TfW6sn1meGvO3ZrVD4TjSCsPyzzW-JPAcdP4&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>[binary data]</pre>
