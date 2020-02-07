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
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1ODA4OTE1MjQsInN1YiI6NDI3LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.RDM-lFuCsUYufr6wBwdkDyxI4-ai1xXpBwulZcIFIIM</pre>

#### Route

<pre>POST /api/v1/user/bonuses/64/comments</pre>

#### Body

<pre>{"data":{"id":"commenttext","type":"comment-texts","attributes":{"text":"+4 Nemo aut possimus sapiente. #officia-voluptatum-accusamus #saepe-repudiandae-officia"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.flts.tk/api/v1/user/bonuses/64/comments&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;commenttext&quot;,&quot;type&quot;:&quot;comment-texts&quot;,&quot;attributes&quot;:{&quot;text&quot;:&quot;+4 Nemo aut possimus sapiente. #officia-voluptatum-accusamus #saepe-repudiandae-officia&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1ODA4OTE1MjQsInN1YiI6NDI3LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.RDM-lFuCsUYufr6wBwdkDyxI4-ai1xXpBwulZcIFIIM&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{
  "data": {
    "id": "64",
    "type": "bonuses",
    "attributes": {
      "text": "+79 to @kling-omar #aliquam-quia-nam Thank you!",
      "points": 79,
      "total-points": 113,
      "created-at": "2020-02-04T08:32:03.995Z"
    },
    "relationships": {
      "sender": {
        "data": {
          "id": "425",
          "type": "users"
        }
      },
      "tags": {
        "data": [
          {
            "id": "517",
            "type": "tags"
          }
        ]
      },
      "comments": {
        "data": [
          {
            "id": "12",
            "type": "comments"
          }
        ]
      },
      "receivers": {
        "data": [
          {
            "id": "426",
            "type": "users"
          }
        ]
      }
    }
  },
  "included": [
    {
      "id": "425",
      "type": "users",
      "attributes": {
        "email": "meria@cartwright.name",
        "full-name": "Coy Yost PhD",
        "username": "yost-phd-coy",
        "profile-image-avatar-url": "memory://user/profile_image/1df94aa20ad2133d805640df6ecb19cc.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "1971-12-20"
      }
    },
    {
      "id": "12",
      "type": "comments",
      "attributes": {
        "created-at": "2020-02-04T08:32:04.135Z",
        "text": "+4 Nemo aut possimus sapiente. #officia-voluptatum-accusamus #saepe-repudiandae-officia"
      },
      "relationships": {
        "bonus": {
          "data": {
            "id": "64",
            "type": "bonuses"
          }
        },
        "sender": {
          "data": {
            "id": "427",
            "type": "users"
          }
        },
        "tags": {
          "data": []
        }
      }
    },
    {
      "id": "427",
      "type": "users",
      "attributes": {
        "email": "clyde@skiles.info",
        "full-name": "Shirl Kuhlman PhD",
        "username": "phd.kuhlman.shirl",
        "profile-image-avatar-url": "memory://user/profile_image/a44dc56ffcb6e57ae02546bd79cda85a.png",
        "bonus-balance": 10000,
        "allowance-balance": 9996,
        "birth-date": "1987-09-18"
      }
    },
    {
      "id": "426",
      "type": "users",
      "attributes": {
        "email": "eloy@trantow.io",
        "full-name": "Omar Kling",
        "username": "kling-omar",
        "profile-image-avatar-url": "memory://user/profile_image/3ca84f5d41e0abfb2c04a5ccb8337000.png",
        "bonus-balance": 10004,
        "allowance-balance": 10000,
        "birth-date": "1986-06-12"
      }
    }
  ]
}</pre>
