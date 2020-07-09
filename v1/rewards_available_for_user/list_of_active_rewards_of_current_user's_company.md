# Rewards available for User API

## List of active rewards of current user&#39;s company

### GET /api/v1/user/rewards
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzUsInN1YiI6MzI1NiwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.-AJvb-DmS6PWwp2PnRTS-Xj1CGVuj9cCoVcdIOF0F4c</pre>

#### Route

<pre>GET /api/v1/user/rewards</pre>

#### Query Parameters

<pre>{}: </pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/rewards&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzUsInN1YiI6MzI1NiwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.-AJvb-DmS6PWwp2PnRTS-Xj1CGVuj9cCoVcdIOF0F4c&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": []
}</pre>
