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
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MjgsInN1YiI6MTkzMCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.iQY9oqAKmhSoY1fRPfZf3UWKF8gc1HNQcNYC5eTpqxI</pre>

#### Route

<pre>POST /api/v1/user/bonuses/304/comments</pre>

#### Body

<pre>{"data":{"id":"commenttext","type":"comment-texts","attributes":{"text":"+33 Dolorem eos ut quia. #sequi-ipsum-ut #repudiandae-minima-sit"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/user/bonuses/304/comments&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;commenttext&quot;,&quot;type&quot;:&quot;comment-texts&quot;,&quot;attributes&quot;:{&quot;text&quot;:&quot;+33 Dolorem eos ut quia. #sequi-ipsum-ut #repudiandae-minima-sit&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MjgsInN1YiI6MTkzMCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.iQY9oqAKmhSoY1fRPfZf3UWKF8gc1HNQcNYC5eTpqxI&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{
  "data": {
    "id": "304",
    "type": "bonuses",
    "attributes": {
      "text": "+21 to @harber.mrs.winfred #et-a-aut Thank you!",
      "points": 21,
      "total-points": 131,
      "created-at": "2021-07-26T09:35:28.221Z"
    },
    "relationships": {
      "sender": {
        "data": {
          "id": "1928",
          "type": "users"
        }
      },
      "tags": {
        "data": [
          {
            "id": "2367",
            "type": "tags"
          }
        ]
      },
      "comments": {
        "data": [
          {
            "id": "22",
            "type": "comments"
          }
        ]
      },
      "receivers": {
        "data": [
          {
            "id": "1929",
            "type": "users"
          }
        ]
      }
    }
  },
  "included": [
    {
      "id": "1928",
      "type": "users",
      "attributes": {
        "email": "marva.marks@bailey.com",
        "full-name": "Kirk Boehm PhD",
        "username": "phd.kirk.boehm",
        "profile-image-avatar-url": "memory://user/profile_image/aee966b3af5de617657d19cbda13e263.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "1972-05-07"
      }
    },
    {
      "id": "22",
      "type": "comments",
      "attributes": {
        "created-at": "2021-07-26T09:35:28.591Z",
        "text": "+33 Dolorem eos ut quia. #sequi-ipsum-ut #repudiandae-minima-sit"
      },
      "relationships": {
        "bonus": {
          "data": {
            "id": "304",
            "type": "bonuses"
          }
        },
        "sender": {
          "data": {
            "id": "1930",
            "type": "users"
          }
        },
        "tags": {
          "data": []
        }
      }
    },
    {
      "id": "1930",
      "type": "users",
      "attributes": {
        "email": "shelton_bogan@emard.com",
        "full-name": "Percy Weber",
        "username": "percy.weber",
        "profile-image-avatar-url": "memory://user/profile_image/f98686df7a1862431ae43fc8e9c460d6.png",
        "bonus-balance": 10000,
        "allowance-balance": 9967,
        "birth-date": "1981-04-05"
      }
    },
    {
      "id": "1929",
      "type": "users",
      "attributes": {
        "email": "winston@hilll.net",
        "full-name": "Mrs. Winfred Harber",
        "username": "harber.mrs.winfred",
        "profile-image-avatar-url": "memory://user/profile_image/a43fdfeb7ece27a21e77972088d107c7.png",
        "bonus-balance": 10033,
        "allowance-balance": 10000,
        "birth-date": "2017-03-30"
      }
    }
  ]
}</pre>
