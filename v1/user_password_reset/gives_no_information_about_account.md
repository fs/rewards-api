# User Password Reset API

## gives no information about account

### POST /api/v1/user/password_reset

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| email | Email | false |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json</pre>

#### Route

<pre>POST /api/v1/user/password_reset</pre>

#### Body

<pre>{"data":{"id":"passwordresetrequest","type":"password-reset-requests","attributes":{"email":"test@test.com"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/user/password_reset&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;passwordresetrequest&quot;,&quot;type&quot;:&quot;password-reset-requests&quot;,&quot;attributes&quot;:{&quot;email&quot;:&quot;test@test.com&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot;</pre>

### Response

#### Headers

<pre></pre>

#### Status

<pre>204 No Content</pre>

