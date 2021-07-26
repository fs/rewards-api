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

<pre>{"data":{"id":"userrefreshtokenrequest","type":"user-refresh-token-requests","attributes":{"refresh-token":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzIsInN1YiI6MTk0OCwidHlwZSI6InJlZnJlc2giLCJjbGllbnRfaWQiOiIyIn0.FNZR8T_sEHPQ6yf6GcmdJp066twgsN3sLF-6VkEyME4"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/user/tokens&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;userrefreshtokenrequest&quot;,&quot;type&quot;:&quot;user-refresh-token-requests&quot;,&quot;attributes&quot;:{&quot;refresh-token&quot;:&quot;eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzIsInN1YiI6MTk0OCwidHlwZSI6InJlZnJlc2giLCJjbGllbnRfaWQiOiIyIn0.FNZR8T_sEHPQ6yf6GcmdJp066twgsN3sLF-6VkEyME4&quot;}}}&#39; -X PUT \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{
  "data": {
    "id": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzIsInN1YiI6MTk0OCwidHlwZSI6ImFjY2VzcyJ9.CePsoopScaf_h3wCxLC794roAdk96gh9F0uSh4AGQWY",
    "type": "paired-jwt-tokens",
    "attributes": {
      "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzIsInN1YiI6MTk0OCwidHlwZSI6ImFjY2VzcyJ9.CePsoopScaf_h3wCxLC794roAdk96gh9F0uSh4AGQWY",
      "refresh": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MzI0NzYxMzIsInN1YiI6MTk0OCwidHlwZSI6InJlZnJlc2giLCJjbGllbnRfaWQiOiIyIn0.JYad1F7qg3Q20turV9U5Uy0bye4TI8JsJXHf-VV1GGE"
    }
  }
}</pre>
