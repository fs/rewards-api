# User Tokens API

## Create User Token

### POST /api/v1/user/tokens

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| email | User email | true |  |
| password | User password | true |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json</pre>

#### Route

<pre>POST /api/v1/user/tokens</pre>

#### Body

<pre>{"data":{"type":"user-token-requests","attributes":{"email":"user@example.com","password":"123456"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.flts.tk/api/v1/user/tokens&quot; -d &#39;{&quot;data&quot;:{&quot;type&quot;:&quot;user-token-requests&quot;,&quot;attributes&quot;:{&quot;email&quot;:&quot;user@example.com&quot;,&quot;password&quot;:&quot;123456&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{"data":{"id":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzQsInN1YiI6Mjg5fQ.sYwR1gp9pQ9zFwWeWuk88IG4zzxJ-fsm0nlrV9u208w","type":"jwt-tokens","attributes":{"token":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzQsInN1YiI6Mjg5fQ.sYwR1gp9pQ9zFwWeWuk88IG4zzxJ-fsm0nlrV9u208w"}}}</pre>
