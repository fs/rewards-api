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
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MjksInN1YiI6NjAsInR5cGUiOiJhY2Nlc3MiLCJjbGllbnRfaWQiOiIyIn0.DcTHF57AMg88XavmuJb6FiwkdbuAMEq7g6JUItyXwTs</pre>

#### Route

<pre>POST /api/v1/bot/bonuses</pre>

#### Body

<pre>{"data":{"id":"bonustext","type":"bonus-texts","attributes":{"text":"+88 to @strosin-wilfred @angelo_morissette #est-nulla-provident #et-exercitationem-molestias Thank you!"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/bot/bonuses&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;bonustext&quot;,&quot;type&quot;:&quot;bonus-texts&quot;,&quot;attributes&quot;:{&quot;text&quot;:&quot;+88 to @strosin-wilfred @angelo_morissette #est-nulla-provident #et-exercitationem-molestias Thank you!&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MjksInN1YiI6NjAsInR5cGUiOiJhY2Nlc3MiLCJjbGllbnRfaWQiOiIyIn0.DcTHF57AMg88XavmuJb6FiwkdbuAMEq7g6JUItyXwTs&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{
  "data": {
    "id": "307",
    "type": "bonuses",
    "attributes": {
      "text": "+88 to @strosin-wilfred @angelo_morissette #est-nulla-provident #et-exercitationem-molestias Thank you!",
      "points": 88,
      "total-points": 88,
      "created-at": "2021-07-26T09:35:29.684Z"
    },
    "relationships": {
      "sender": {
        "data": {
          "id": "60",
          "type": "bots"
        }
      },
      "tags": {
        "data": [
          {
            "id": "2375",
            "type": "tags"
          },
          {
            "id": "2376",
            "type": "tags"
          }
        ]
      },
      "comments": {
        "data": []
      },
      "receivers": {
        "data": [
          {
            "id": "1937",
            "type": "users"
          },
          {
            "id": "1938",
            "type": "users"
          }
        ]
      }
    }
  },
  "included": [
    {
      "id": "60",
      "type": "bots",
      "attributes": {
        "name": "myles_stiedemann"
      }
    }
  ]
}</pre>
