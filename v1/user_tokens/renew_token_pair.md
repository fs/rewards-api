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

<pre>{"data":{"id":"userrefreshtokenrequest","type":"user-refresh-token-requests","attributes":{"refresh-token":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzMsInN1YiI6MzI0OSwidHlwZSI6InJlZnJlc2giLCJjbGllbnRfaWQiOiIyIn0.2jNPQCB03jHMN9Yz4obso4DwgqzFepC3rhh8Vx8xsG0"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/user/tokens&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;userrefreshtokenrequest&quot;,&quot;type&quot;:&quot;user-refresh-token-requests&quot;,&quot;attributes&quot;:{&quot;refresh-token&quot;:&quot;eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzMsInN1YiI6MzI0OSwidHlwZSI6InJlZnJlc2giLCJjbGllbnRfaWQiOiIyIn0.2jNPQCB03jHMN9Yz4obso4DwgqzFepC3rhh8Vx8xsG0&quot;}}}&#39; -X PUT \
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
    "id": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzMsInN1YiI6MzI0OSwidHlwZSI6ImFjY2VzcyJ9.6fEySlWJxiL64-ZGYpK7hqUmpg4lPNNqrowfUN4pZDA",
    "type": "paired-jwt-tokens",
    "attributes": {
      "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzMsInN1YiI6MzI0OSwidHlwZSI6ImFjY2VzcyJ9.6fEySlWJxiL64-ZGYpK7hqUmpg4lPNNqrowfUN4pZDA",
      "refresh": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTk0Njc2NzMsInN1YiI6MzI0OSwidHlwZSI6InJlZnJlc2giLCJjbGllbnRfaWQiOiIyIn0.O88L5M-CIsqTeBY1o18RKu36EsvDNvhud1ittJDPSRE"
    }
  }
}</pre>
