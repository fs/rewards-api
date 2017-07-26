# Bot Bonuses API

## Create bonus

### POST /api/v1/bot/bonuses

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| text | Bonus text | true |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MDExNTIxNTIsInN1YiI6OTR9.mNbjdEHOTSuMn2H2_Na-uFpPdY45b3WuroIIXB6zYek</pre>

#### Route

<pre>POST /api/v1/bot/bonuses</pre>

#### Body

<pre>{"data":{"id":"bonus-text","type":"bonus-texts","attributes":{"text":"+69 to @kulas.lou #magni-nisi-sunt Thank you!"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.flts.tk/api/v1/bot/bonuses&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;bonus-text&quot;,&quot;type&quot;:&quot;bonus-texts&quot;,&quot;attributes&quot;:{&quot;text&quot;:&quot;+69 to @kulas.lou #magni-nisi-sunt Thank you!&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MDExNTIxNTIsInN1YiI6OTR9.mNbjdEHOTSuMn2H2_Na-uFpPdY45b3WuroIIXB6zYek&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{"data":{"id":"68","type":"bonuses","attributes":{"text":"+69 to @kulas.lou #magni-nisi-sunt Thank you!","points":69}}}</pre>
