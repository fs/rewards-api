# User Bonuses API

## List bonuses

### GET /api/v1/user/bonuses
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzMsInN1YiI6MzI0MCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.uYYCHl8TIUkt8FGFP6HoV3RIlqcvYzGf21jxsylCmyo</pre>

#### Route

<pre>GET /api/v1/user/bonuses</pre>

#### Query Parameters

<pre>{}: </pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/bonuses&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzMsInN1YiI6MzI0MCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.uYYCHl8TIUkt8FGFP6HoV3RIlqcvYzGf21jxsylCmyo&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": [
    {
      "id": "627",
      "type": "bonuses",
      "attributes": {
        "text": "+28 to @jerry_mccullough #ea-dolor-dolor Thank you!",
        "points": 28,
        "total-points": 128,
        "created-at": "2020-07-09T08:34:33.068Z"
      },
      "relationships": {
        "sender": {
          "data": {
            "id": "3238",
            "type": "users"
          }
        },
        "tags": {
          "data": [
            {
              "id": "4128",
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
              "id": "3239",
              "type": "users"
            }
          ]
        }
      }
    },
    {
      "id": "626",
      "type": "bonuses",
      "attributes": {
        "text": "+1 to @ruecker_yung #voluptas-optio-fugiat Thank you!",
        "points": 1,
        "total-points": 97,
        "created-at": "2020-07-09T08:34:32.994Z"
      },
      "relationships": {
        "sender": {
          "data": {
            "id": "3236",
            "type": "users"
          }
        },
        "tags": {
          "data": [
            {
              "id": "4127",
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
              "id": "3237",
              "type": "users"
            }
          ]
        }
      }
    }
  ],
  "included": [
    {
      "id": "3238",
      "type": "users",
      "attributes": {
        "email": "deloise.hermann@gerlach.com",
        "full-name": "Faustino Nienow V",
        "username": "nienow_v_faustino",
        "profile-image-avatar-url": "memory://user/profile_image/a8825d50be9050362cf116baa55d437c.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "1992-12-27"
      }
    },
    {
      "id": "4128",
      "type": "tags",
      "attributes": {
        "label": "ea-dolor-dolor"
      }
    },
    {
      "id": "3239",
      "type": "users",
      "attributes": {
        "email": "tyson_abbott@predovicswift.name",
        "full-name": "Jerry McCullough",
        "username": "jerry_mccullough",
        "profile-image-avatar-url": "memory://user/profile_image/01dfed04d95d2771e689100a082352be.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "2008-08-21"
      }
    },
    {
      "id": "3236",
      "type": "users",
      "attributes": {
        "email": "sarita_feeney@ratkewaelchi.com",
        "full-name": "Orville Hackett",
        "username": "orville.hackett",
        "profile-image-avatar-url": "memory://user/profile_image/205f1adf932438b5150758710f618cef.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "2002-07-31"
      }
    },
    {
      "id": "4127",
      "type": "tags",
      "attributes": {
        "label": "voluptas-optio-fugiat"
      }
    },
    {
      "id": "3237",
      "type": "users",
      "attributes": {
        "email": "xavier.anderson@roweferry.com",
        "full-name": "Yung Ruecker",
        "username": "ruecker_yung",
        "profile-image-avatar-url": "memory://user/profile_image/ec0e5073d9f91adaacc2c93bbf73e111.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "1971-01-23"
      }
    }
  ],
  "links": {
    "self": "http://example.org/api/v1/user/bonuses?%7B%7D=&page%5Bnumber%5D=1&page%5Bsize%5D=10",
    "first": "http://example.org/api/v1/user/bonuses?%7B%7D=&page%5Bnumber%5D=1&page%5Bsize%5D=10",
    "prev": null,
    "next": null,
    "last": "http://example.org/api/v1/user/bonuses?%7B%7D=&page%5Bnumber%5D=1&page%5Bsize%5D=10"
  }
}</pre>
