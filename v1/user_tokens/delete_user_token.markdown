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
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1NDg0OTI0NDksInN1YiI6MjQwMzUsInR5cGUiOiJhY2Nlc3MiLCJjbGllbnRfaWQiOiIyIn0.zxDkJwwzjtyaKVoKcmLs_sCdp44XqIS67p52brA3T2g</pre>

#### Route

<pre>DELETE /api/v1/user/tokens</pre>

#### Body

<pre>{"data":{"id":"userrefreshtokenrequest","type":"user-refresh-token-requests","attributes":{"refresh-token":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1NDg0OTI0NDksInN1YiI6MjQwMzUsInR5cGUiOiJyZWZyZXNoIiwiY2xpZW50X2lkIjoiMiJ9.8NRwW6we2vwJ5V0jS0us-3usezu0bUwtpjzHikEA-PU"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.flts.tk/api/v1/user/tokens&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;userrefreshtokenrequest&quot;,&quot;type&quot;:&quot;user-refresh-token-requests&quot;,&quot;attributes&quot;:{&quot;refresh-token&quot;:&quot;eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1NDg0OTI0NDksInN1YiI6MjQwMzUsInR5cGUiOiJyZWZyZXNoIiwiY2xpZW50X2lkIjoiMiJ9.8NRwW6we2vwJ5V0jS0us-3usezu0bUwtpjzHikEA-PU&quot;}}}&#39; -X DELETE \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1NDg0OTI0NDksInN1YiI6MjQwMzUsInR5cGUiOiJhY2Nlc3MiLCJjbGllbnRfaWQiOiIyIn0.zxDkJwwzjtyaKVoKcmLs_sCdp44XqIS67p52brA3T2g&quot;</pre>

### Response

#### Headers

<pre></pre>

#### Status

<pre>204 No Content</pre>

