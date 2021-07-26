# Rewards available for User API

## List of active rewards of current user&#39;s company

### GET /api/v1/user/rewards
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzYsInN1YiI6MTk4MywidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.XZxUCE5XksRVBaOf1QezypMA0UOR9Wvo0hMXOt_ev1o</pre>

#### Route

<pre>GET /api/v1/user/rewards</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/rewards&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzYsInN1YiI6MTk4MywidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.XZxUCE5XksRVBaOf1QezypMA0UOR9Wvo0hMXOt_ev1o&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": []
}</pre>
