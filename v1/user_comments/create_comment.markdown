# User Comments API

## Create comment

### POST /api/v1/user/bonuses/:bonus_id/comments

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| text | Comment text | true |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzMsInN1YiI6MjgyfQ.pEEOWGb8M5zpjIj3x5EXr5zz5qAS7ZQHyAFCWxrHp3k</pre>

#### Route

<pre>POST /api/v1/user/bonuses/47/comments</pre>

#### Body

<pre>{"data":{"type":"comment-texts","attributes":{"text":"+62 Voluptas accusamus repudiandae quibusdam aut temporibus. #consequatur-qui-magni"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.flts.tk/api/v1/user/bonuses/47/comments&quot; -d &#39;{&quot;data&quot;:{&quot;type&quot;:&quot;comment-texts&quot;,&quot;attributes&quot;:{&quot;text&quot;:&quot;+62 Voluptas accusamus repudiandae quibusdam aut temporibus. #consequatur-qui-magni&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzMsInN1YiI6MjgyfQ.pEEOWGb8M5zpjIj3x5EXr5zz5qAS7ZQHyAFCWxrHp3k&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{"data":{"id":"47","type":"bonuses","attributes":{"text":"+11 to @kamron-mcdermott #quia-saepe-molestiae Thank you!","points":11,"total-points":157,"created-at":"2017-11-16T12:31:13.784Z"},"relationships":{"sender":{"data":{"id":"280","type":"users"}},"comments":{"data":[{"id":"10","type":"comments"}]}}},"included":[{"id":"10","type":"comments","attributes":{"created-at":"2017-11-16T12:31:13.904Z","text":"+62 Voluptas accusamus repudiandae quibusdam aut temporibus. #consequatur-qui-magni"},"relationships":{"bonus":{"data":{"id":"47","type":"bonuses"}},"sender":{"data":{"id":"282","type":"users"}}}}]}</pre>
