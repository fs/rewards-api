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

<pre>{"data":{"type":"user-token-requests","attributes":{"email":"user@example.com","password":"123456","client-id":"c7f160ea-fd3c-4e76-97b1-e0a2eafa5a70"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/user/tokens&quot; -d &#39;{&quot;data&quot;:{&quot;type&quot;:&quot;user-token-requests&quot;,&quot;attributes&quot;:{&quot;email&quot;:&quot;user@example.com&quot;,&quot;password&quot;:&quot;123456&quot;,&quot;client-id&quot;:&quot;c7f160ea-fd3c-4e76-97b1-e0a2eafa5a70&quot;}}}&#39; -X POST \
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
    "id": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzEsInN1YiI6MTk0NCwidHlwZSI6ImFjY2VzcyJ9.yXKECKqUzp1uM83iENQEYOy0zLQm-nqizv0PXzaFRLc",
    "type": "paired-jwt-tokens",
    "attributes": {
      "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzEsInN1YiI6MTk0NCwidHlwZSI6ImFjY2VzcyJ9.yXKECKqUzp1uM83iENQEYOy0zLQm-nqizv0PXzaFRLc",
      "refresh": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MzI0NzYxMzEsInN1YiI6MTk0NCwidHlwZSI6InJlZnJlc2giLCJjbGllbnRfaWQiOiJjN2YxNjBlYS1mZDNjLTRlNzYtOTdiMS1lMGEyZWFmYTVhNzAifQ.olkEUeb1mG9HZ5qZ90mmG30TDUmk332qqLr0FPib2Mo"
    }
  }
}</pre>
