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
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzUsInN1YiI6OTUsInR5cGUiOiJhY2Nlc3MiLCJjbGllbnRfaWQiOiIyIn0.AnL0Y3Pn_0RkWiZALxxWTPwEFcp6m6zDnmQRRxyZAU4</pre>

#### Route

<pre>POST /api/v1/bot/bonuses</pre>

#### Body

<pre>{"data":{"id":"bonustext","type":"bonus-texts","attributes":{"text":"+47 to @dr-sharee-romaguera @rutherford_beulah_ii #sequi-hic-ea #et-qui-illo Thank you!"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/bot/bonuses&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;bonustext&quot;,&quot;type&quot;:&quot;bonus-texts&quot;,&quot;attributes&quot;:{&quot;text&quot;:&quot;+47 to @dr-sharee-romaguera @rutherford_beulah_ii #sequi-hic-ea #et-qui-illo Thank you!&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzUsInN1YiI6OTUsInR5cGUiOiJhY2Nlc3MiLCJjbGllbnRfaWQiOiIyIn0.AnL0Y3Pn_0RkWiZALxxWTPwEFcp6m6zDnmQRRxyZAU4&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{
  "data": {
    "id": "632",
    "type": "bonuses",
    "attributes": {
      "text": "+47 to @dr-sharee-romaguera @rutherford_beulah_ii #sequi-hic-ea #et-qui-illo Thank you!",
      "points": 47,
      "total-points": 47,
      "created-at": "2020-07-09T08:34:35.597Z"
    },
    "relationships": {
      "sender": {
        "data": {
          "id": "95",
          "type": "bots"
        }
      },
      "tags": {
        "data": [
          {
            "id": "4149",
            "type": "tags"
          },
          {
            "id": "4148",
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
            "id": "3257",
            "type": "users"
          },
          {
            "id": "3258",
            "type": "users"
          }
        ]
      }
    }
  },
  "included": [
    {
      "id": "95",
      "type": "bots",
      "attributes": {
        "name": "vernetta"
      }
    }
  ]
}</pre>
