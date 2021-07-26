# User Tokens API

## Delete User Token

### DELETE /api/v1/user/tokens

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| refresh_token | Valid refresh token | true |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzEsInN1YiI6MTk0MywidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.h3i3fqWa6XvAyvASQSs-pROC1FXU_bhdpDA7K7EZQa8</pre>

#### Route

<pre>DELETE /api/v1/user/tokens</pre>

#### Body

<pre>{"data":{"id":"userrefreshtokenrequest","type":"user-refresh-token-requests","attributes":{"refresh-token":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzEsInN1YiI6MTk0MywidHlwZSI6InJlZnJlc2giLCJjbGllbnRfaWQiOiIyIn0.sbAWDWt87cqvcq_t6lmCASiaZX-riBb6yQToAbRQzvg"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/user/tokens&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;userrefreshtokenrequest&quot;,&quot;type&quot;:&quot;user-refresh-token-requests&quot;,&quot;attributes&quot;:{&quot;refresh-token&quot;:&quot;eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzEsInN1YiI6MTk0MywidHlwZSI6InJlZnJlc2giLCJjbGllbnRfaWQiOiIyIn0.sbAWDWt87cqvcq_t6lmCASiaZX-riBb6yQToAbRQzvg&quot;}}}&#39; -X DELETE \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzEsInN1YiI6MTk0MywidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.h3i3fqWa6XvAyvASQSs-pROC1FXU_bhdpDA7K7EZQa8&quot;</pre>

### Response

#### Headers

<pre></pre>

#### Status

<pre>204 No Content</pre>

