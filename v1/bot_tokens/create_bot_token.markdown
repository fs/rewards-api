# Bot Tokens API

## Create Bot Token

### POST /api/v1/bot/tokens

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| name | Bot name | true |  |
| password | Bot password | true |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json</pre>

#### Route

<pre>POST /api/v1/bot/tokens</pre>

#### Body

<pre>{"data":{"id":"bottokenrequest","type":"bot-token-requests","attributes":{"name":"example","password":"123456"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.flts.tk/api/v1/bot/tokens&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;bottokenrequest&quot;,&quot;type&quot;:&quot;bot-token-requests&quot;,&quot;attributes&quot;:{&quot;name&quot;:&quot;example&quot;,&quot;password&quot;:&quot;123456&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{"data":{"id":"jwt-token","type":"jwt-tokens","attributes":{"token":"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MDExNTIxNTMsInN1YiI6OTV9.hIe-OW-GGxpwOAtBTJU4H6JA6Zdt_Fzmm7MxUHCW9vw"}}}</pre>
