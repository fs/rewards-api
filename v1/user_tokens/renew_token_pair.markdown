# User Tokens API

## Renew Token Pair

### PUT /api/v1/user/tokens

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| refresh_token | Valid refresh token | true |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json</pre>

#### Route

<pre>PUT /api/v1/user/tokens</pre>

#### Body

<pre>{"data":{"id":"userrefreshtokenrequest","type":"user-refresh-token-requests","attributes":{"refresh-token":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1NDg0OTI0NDksInN1YiI6MjQwMzksInR5cGUiOiJyZWZyZXNoIiwiY2xpZW50X2lkIjoiMiJ9.vm2UoQKnH4jW3wC7a7hQKJIFrgvgm_0_47mYRco_fnQ"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.flts.tk/api/v1/user/tokens&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;userrefreshtokenrequest&quot;,&quot;type&quot;:&quot;user-refresh-token-requests&quot;,&quot;attributes&quot;:{&quot;refresh-token&quot;:&quot;eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1NDg0OTI0NDksInN1YiI6MjQwMzksInR5cGUiOiJyZWZyZXNoIiwiY2xpZW50X2lkIjoiMiJ9.vm2UoQKnH4jW3wC7a7hQKJIFrgvgm_0_47mYRco_fnQ&quot;}}}&#39; -X PUT \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{"data":{"id":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1NDg0OTI0NDksInN1YiI6MjQwMzksInR5cGUiOiJhY2Nlc3MifQ.nyl66YYb4PTMRX9TsT8oqrT8PL6R_mYlDxhBMBEXovM","type":"paired-jwt-tokens","attributes":{"token":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1NDg0OTI0NDksInN1YiI6MjQwMzksInR5cGUiOiJhY2Nlc3MifQ.nyl66YYb4PTMRX9TsT8oqrT8PL6R_mYlDxhBMBEXovM","refresh":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1NTM1OTAwNDksInN1YiI6MjQwMzksInR5cGUiOiJyZWZyZXNoIiwiY2xpZW50X2lkIjoiMiJ9.ylDr47YNmLq38xuLIUg3xmDSj61CmLD5dJkxBdBIKj4"}}}</pre>
