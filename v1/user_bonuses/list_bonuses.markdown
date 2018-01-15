# User Bonuses API

## List bonuses

### GET /api/v1/user/bonuses
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzMsInN1YiI6Mjc0fQ.E9QHRo7JSOSJxohX01VtQr7g7YYrP4pTa3GcDPPG2x8</pre>

#### Route

<pre>GET /api/v1/user/bonuses</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.flts.tk/api/v1/user/bonuses&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1MTA5MjE4NzMsInN1YiI6Mjc0fQ.E9QHRo7JSOSJxohX01VtQr7g7YYrP4pTa3GcDPPG2x8&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": [
    {
      "id": "25",
      "type": "bonuses",
      "attributes": {
        "text": "+100 @phd.dortha.bruen thank you #doloribus-nulla-dicta ",
        "points": 100,
        "total-points": 238,
        "created-at": "2018-01-08T07:05:40.666Z"
      },
      "relationships": {
        "sender": {
          "data": {
            "id": "12",
            "type": "users"
          }
        },
        "comments": {
          "data": [
            {
              "id": "63",
              "type": "comments"
            }
          ]
        }
      }
    }
  ],
  "included": [
    {
      "id": "12",
      "type": "users",
      "attributes": {
        "full-name": "Constantin Pacocha"
      }
    },
    {
      "id": "63",
      "type": "comments",
      "attributes": {
        "created-at": "2018-01-08T07:06:56.304Z",
        "text": "+69 to @phd.dortha.bruen #sed-nulla-quasi Thank you!"
      },
      "relationships": {
        "bonus": {
          "data": {
            "id": "25",
            "type": "bonuses"
          }
        },
        "sender": {
          "data": {
            "id": "11",
            "type": "users"
          }
        }
      }
    },
    {
      "id": "11",
      "type": "users",
      "attributes": {
        "full-name": "Malcolm Ankunding III"
      }
    }
  ],
  "links": {
    "self": "http:\/\/localhost:5000\/api\/v1\/user\/bonuses?page%5Bnumber%5D=1&page%5Bsize%5D=10",
    "first": "http:\/\/localhost:5000\/api\/v1\/user\/bonuses?page%5Bnumber%5D=1&page%5Bsize%5D=10",
    "prev": null,
    "next": null,
    "last": "http:\/\/localhost:5000\/api\/v1\/user\/bonuses?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  }
}</pre>
