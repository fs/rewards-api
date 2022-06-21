# Received User Bonuses API

## List recieved for current user bonuses

### GET /api/v1/user/received_user_bonuses
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2NTU5MDI1OTcsInN1YiI6ODc1LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.h71v0Ig1VliKhijlFBKc41-FNfK_MwGN3jwCqX-4mvo</pre>

#### Route

<pre>GET /api/v1/user/received_user_bonuses</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/received_user_bonuses&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2NTU5MDI1OTcsInN1YiI6ODc1LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.h71v0Ig1VliKhijlFBKc41-FNfK_MwGN3jwCqX-4mvo&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": [
    {
      "id": "341",
      "type": "bonuses",
      "attributes": {
        "text": "+9 to @dach.jefferson #impedit-error-doloribus Thank you!",
        "points": 9,
        "total-points": 83,
        "created-at": "2022-06-21T12:56:37.334Z"
      },
      "relationships": {
        "sender": {
          "data": {
            "id": "877",
            "type": "users"
          }
        },
        "tags": {
          "data": [
            {
              "id": "990",
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
              "id": "875",
              "type": "users"
            }
          ]
        }
      }
    },
    {
      "id": "340",
      "type": "bonuses",
      "attributes": {
        "text": "+62 to @dach.jefferson #unde-nostrum-aliquam Thank you!",
        "points": 62,
        "total-points": 82,
        "created-at": "2022-06-21T12:56:37.308Z"
      },
      "relationships": {
        "sender": {
          "data": {
            "id": "876",
            "type": "users"
          }
        },
        "tags": {
          "data": [
            {
              "id": "989",
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
              "id": "875",
              "type": "users"
            }
          ]
        }
      }
    }
  ],
  "links": {
    "self": "http://example.org/api/v1/user/received_user_bonuses?page%5Bnumber%5D=1&page%5Bsize%5D=10",
    "first": "http://example.org/api/v1/user/received_user_bonuses?page%5Bnumber%5D=1&page%5Bsize%5D=10",
    "prev": null,
    "next": null,
    "last": "http://example.org/api/v1/user/received_user_bonuses?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  }
}</pre>
