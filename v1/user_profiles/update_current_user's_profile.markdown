# User Profiles API

## Update current user&#39;s profile

### PATCH /api/v1/user/profile

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| full_name | Full Name | false |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTM1MTE1NzUsInN1YiI6NDA3LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.4Cp_bjgohC-LLXSRYoh3hcYvkdpmv84KS6ymvK4WI7U</pre>

#### Route

<pre>PATCH /api/v1/user/profile</pre>

#### Body

<pre>{"data":{"id":"updateprofilerequest","type":"update-profile-requests","attributes":{"full-name":"New Full Name"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.flts.tk/api/v1/user/profile&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;updateprofilerequest&quot;,&quot;type&quot;:&quot;update-profile-requests&quot;,&quot;attributes&quot;:{&quot;full-name&quot;:&quot;New Full Name&quot;}}}&#39; -X PATCH \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTM1MTE1NzUsInN1YiI6NDA3LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.4Cp_bjgohC-LLXSRYoh3hcYvkdpmv84KS6ymvK4WI7U&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>[binary data]</pre>
