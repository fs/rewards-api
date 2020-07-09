# Users Rewards API

## List of users_rewards of current user

### GET /api/v1/user/users_rewards
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzcsInN1YiI6MzI2OCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.ctZt7_s02HM4AZKEw1I7hIcMryho0puupfhgJGt5Eks</pre>

#### Route

<pre>GET /api/v1/user/users_rewards</pre>

#### Query Parameters

<pre>{}: </pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/users_rewards&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzcsInN1YiI6MzI2OCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.ctZt7_s02HM4AZKEw1I7hIcMryho0puupfhgJGt5Eks&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": []
}</pre>
