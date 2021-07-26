# Rewards owned by User API

## List of users_rewards of current user

### GET /api/v1/user/users_rewards
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzUsInN1YiI6MTk3OCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.Kt6PfB08XW9dmPax87pP1_x4uF0p2H18eT6wObDYXz4</pre>

#### Route

<pre>GET /api/v1/user/users_rewards</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/users_rewards&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzUsInN1YiI6MTk3OCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.Kt6PfB08XW9dmPax87pP1_x4uF0p2H18eT6wObDYXz4&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": []
}</pre>
