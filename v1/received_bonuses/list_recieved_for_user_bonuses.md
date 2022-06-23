# Received Bonuses API

## List recieved for user bonuses

### GET /api/v1/user/users/:user_id/received_bonuses
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2NTYwODYwMjgsInN1YiI6MTU0NSwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.kZ3yZOWaDsZ758gc_e-CNTsfIqH1ixWkb5m3akOq0kQ</pre>

#### Route

<pre>GET /api/v1/user/users/1542/received_bonuses</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/users/1542/received_bonuses&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2NTYwODYwMjgsInN1YiI6MTU0NSwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.kZ3yZOWaDsZ758gc_e-CNTsfIqH1ixWkb5m3akOq0kQ&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": [
    {
      "id": "557",
      "type": "bonuses",
      "attributes": {
        "text": "+6 to @shane_rohan #laudantium-voluptates-odio Thank you!",
        "points": 6,
        "total-points": 48,
        "created-at": "2022-06-23T15:53:48.668Z"
      },
      "relationships": {
        "sender": {
          "data": {
            "id": "1544",
            "type": "users"
          }
        },
        "tags": {
          "data": [
            {
              "id": "1846",
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
              "id": "1542",
              "type": "users"
            }
          ]
        }
      }
    },
    {
      "id": "556",
      "type": "bonuses",
      "attributes": {
        "text": "+38 to @shane_rohan #voluptatem-enim-voluptas Thank you!",
        "points": 38,
        "total-points": 132,
        "created-at": "2022-06-23T15:53:48.643Z"
      },
      "relationships": {
        "sender": {
          "data": {
            "id": "1543",
            "type": "users"
          }
        },
        "tags": {
          "data": [
            {
              "id": "1845",
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
              "id": "1542",
              "type": "users"
            }
          ]
        }
      }
    }
  ],
  "links": {
    "self": "http://example.org/api/v1/user/users/1542/received_bonuses?page%5Bnumber%5D=1&page%5Bsize%5D=10",
    "first": "http://example.org/api/v1/user/users/1542/received_bonuses?page%5Bnumber%5D=1&page%5Bsize%5D=10",
    "prev": null,
    "next": null,
    "last": "http://example.org/api/v1/user/users/1542/received_bonuses?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  }
}</pre>
