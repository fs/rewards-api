# User Bonuses API

## Create bonus

### POST /api/v1/user/bonuses

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| text | Bonus text | true |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzMsInN1YiI6MjY4fQ.8-Kd2k4mLwFCDG5-I7AYLeOlLT7p0Y9ChbyfArtH6J0</pre>

#### Route

<pre>POST /api/v1/user/bonuses</pre>

#### Body

<pre>{"data":{"type":"bonus-texts","attributes":{"text":"+45 to @mcdermott_phd_fiona #animi-odit-porro Thank you!"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.flts.tk/api/v1/user/bonuses&quot; -d &#39;{&quot;data&quot;:{&quot;type&quot;:&quot;bonus-texts&quot;,&quot;attributes&quot;:{&quot;text&quot;:&quot;+45 to @mcdermott_phd_fiona #animi-odit-porro Thank you!&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzMsInN1YiI6MjY4fQ.8-Kd2k4mLwFCDG5-I7AYLeOlLT7p0Y9ChbyfArtH6J0&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{"data":{"id":"42","type":"bonuses","attributes":{"text":"+45 to @mcdermott_phd_fiona #animi-odit-porro Thank you!","points":45,"total-points":45,"created-at":"2017-11-16T12:31:13.135Z"},"relationships":{"sender":{"data":{"id":"268","type":"users"}},"comments":{"data":[]}}}}</pre>
