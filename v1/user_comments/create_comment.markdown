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

<pre>{
  "data": {
    "id": "25",
    "type": "bonuses",
    "attributes": {
      "text": "+100 @phd.dortha.bruen thank you #doloribus-nulla-dicta ",
      "points": 100,
      "total-points": 307,
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
            "id": "64",
            "type": "comments"
          }
        ]
      }
    }
  },
  "included": [
    {
      "id": "12",
      "type": "users",
      "attributes": {
        "email": "constantin.pacocha@flatstack.com",
        "full-name": "Constantin Pacocha",
        "username": "constantin.pacocha",
        "profile-image-avatar-url": "\/\/localhost:5000\/assets\/default-user-profile_image-8840d077a11aa734bcdd9e3d58eed663c3262440203b2560bd22ca39d72e14bf.svg",
        "allowance-balance": 4850
      }
    },
    {
      "id": "64",
      "type": "comments",
      "attributes": {
        "created-at": "2018-01-08T07:15:13.759Z",
        "text": "+69 to @phd.dortha.brue #sed-nulla-quasi Thank you!"
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
        "email": "malcolm_ankunding@example.com",
        "full-name": "Malcolm Ankunding III",
        "username": "malcolm_ankunding",
        "profile-image-avatar-url": "https:\/\/fs-rewards-development.s3.eu-central-1.amazonaws.com\/cache\/user\/profile_image\/6a03c171511ed099e7e3b6f564be286d.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIJWLCQQNSWJW7QQA%2F20180108%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20180108T071513Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=5c4f5a439b7851dd93c4f8476d673738cc2a5e66e7259c3eb02cd45eb5a41903",
        "allowance-balance": 9241
      }
    }
  ]
}</pre>
