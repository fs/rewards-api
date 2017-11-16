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
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzQsInN1YiI6MTh9.CpR_DAxCJ6LG8sq5UI2zUC01W-DsgJ0K6hFpKPnH6Tc</pre>

#### Route

<pre>POST /api/v1/bot/bonuses</pre>

#### Body

<pre>{"data":{"type":"bonus-texts","attributes":{"text":"+95 to @i_jones_nikita #alias-accusamus-beatae Thank you!"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.flts.tk/api/v1/bot/bonuses&quot; -d &#39;{&quot;data&quot;:{&quot;type&quot;:&quot;bonus-texts&quot;,&quot;attributes&quot;:{&quot;text&quot;:&quot;+95 to @i_jones_nikita #alias-accusamus-beatae Thank you!&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzQsInN1YiI6MTh9.CpR_DAxCJ6LG8sq5UI2zUC01W-DsgJ0K6hFpKPnH6Tc&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{"data":{"id":"49","type":"bonuses","attributes":{"text":"+95 to @i_jones_nikita #alias-accusamus-beatae Thank you!","points":95,"total-points":95,"created-at":"2017-11-16T12:31:14.639Z"},"relationships":{"sender":{"data":{"id":"18","type":"bots"}},"comments":{"data":[]}}},"included":[{"id":"18","type":"bots","attributes":{"name":"kylie"}}]}</pre>
