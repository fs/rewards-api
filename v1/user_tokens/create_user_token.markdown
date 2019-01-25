# User Tokens API

## Create User Token

### POST /api/v1/user/tokens

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| email | User email | true |  |
| password | User password | true |  |
| client_id | Client id | false |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json</pre>

#### Route

<pre>POST /api/v1/user/tokens</pre>

#### Body

<pre>{"data":{"type":"user-token-requests","attributes":{"email":"user@example.com","password":"123456","client-id":"2"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.flts.tk/api/v1/user/tokens&quot; -d &#39;{&quot;data&quot;:{&quot;type&quot;:&quot;user-token-requests&quot;,&quot;attributes&quot;:{&quot;email&quot;:&quot;user@example.com&quot;,&quot;password&quot;:&quot;123456&quot;,&quot;client-id&quot;:&quot;2&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{"data":{"id":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1NDg0OTI0NDksInN1YiI6MjQwMzYsInR5cGUiOiJhY2Nlc3MifQ.C_BexThWrOJAXry5eYaseXKULAtIMhvi7Y30oqqMipI","type":"paired-jwt-tokens","attributes":{"token":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1NDg0OTI0NDksInN1YiI6MjQwMzYsInR5cGUiOiJhY2Nlc3MifQ.C_BexThWrOJAXry5eYaseXKULAtIMhvi7Y30oqqMipI","refresh":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1NTM1OTAwNDksInN1YiI6MjQwMzYsInR5cGUiOiJyZWZyZXNoIiwiY2xpZW50X2lkIjoiMiJ9.DGnMvnWbMfsdnk8_EZyLbMOqFlHrjQcfg-MwKRAMncc"}}}</pre>
