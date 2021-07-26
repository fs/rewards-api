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
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzQsInN1YiI6MTk3MywidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.ZjJI2ySj1n9t65QrkaIFBQWPJ-7cjNxrLPisM7zx1Kk</pre>

#### Route

<pre>POST /api/v1/user/bonuses</pre>

#### Body

<pre>{"data":{"id":"bonustext","type":"bonus-texts","attributes":{"text":"+51 to @julian.goyette @wilburn.marks #et-non-adipisci #nesciunt-quia-in Thank you!"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/user/bonuses&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;bonustext&quot;,&quot;type&quot;:&quot;bonus-texts&quot;,&quot;attributes&quot;:{&quot;text&quot;:&quot;+51 to @julian.goyette @wilburn.marks #et-non-adipisci #nesciunt-quia-in Thank you!&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzQsInN1YiI6MTk3MywidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.ZjJI2ySj1n9t65QrkaIFBQWPJ-7cjNxrLPisM7zx1Kk&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{
  "data": {
    "id": "314",
    "type": "bonuses",
    "attributes": {
      "text": "+51 to @julian.goyette @wilburn.marks #et-non-adipisci #nesciunt-quia-in Thank you!",
      "points": 51,
      "total-points": 51,
      "created-at": "2021-07-26T09:35:34.564Z"
    },
    "relationships": {
      "sender": {
        "data": {
          "id": "1973",
          "type": "users"
        }
      },
      "tags": {
        "data": [
          {
            "id": "2407",
            "type": "tags"
          },
          {
            "id": "2408",
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
            "id": "1971",
            "type": "users"
          },
          {
            "id": "1972",
            "type": "users"
          }
        ]
      }
    }
  },
  "included": [
    {
      "id": "1973",
      "type": "users",
      "attributes": {
        "email": "sylvie.wilkinson@hermann.co",
        "full-name": "Meggan Yost",
        "username": "meggan_yost",
        "profile-image-avatar-url": "memory://user/profile_image/806dab7882475364b8ca5f248c2d10b2.png",
        "bonus-balance": 10000,
        "allowance-balance": 9898,
        "birth-date": "2006-07-04"
      }
    },
    {
      "id": "1971",
      "type": "users",
      "attributes": {
        "email": "lawrence@olson.com",
        "full-name": "Julian Goyette",
        "username": "julian.goyette",
        "profile-image-avatar-url": "memory://user/profile_image/ab81236676faac9aa89b8a99cfd7f3f6.png",
        "bonus-balance": 10051,
        "allowance-balance": 10000,
        "birth-date": "2003-12-24"
      }
    },
    {
      "id": "1972",
      "type": "users",
      "attributes": {
        "email": "lan@jerdemcglynn.net",
        "full-name": "Wilburn Marks",
        "username": "wilburn.marks",
        "profile-image-avatar-url": "memory://user/profile_image/ae63eb6ad245aaa0bc07f075c632f191.png",
        "bonus-balance": 10051,
        "allowance-balance": 10000,
        "birth-date": "1972-06-24"
      }
    }
  ]
}</pre>
