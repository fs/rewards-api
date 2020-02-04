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
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1ODA4OTE1MjYsInN1YiI6NDU1LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.U4hM8PPcLQVkzPNhX24_NnJFnStyOmgq2NErky8mUjg</pre>

#### Route

<pre>POST /api/v1/user/bonuses</pre>

#### Body

<pre>{"data":{"id":"bonustext","type":"bonus-texts","attributes":{"text":"+80 to @gabriela_buckridge @don_reinger #magni-quos-ut #non-voluptas-quia Thank you!"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.flts.tk/api/v1/user/bonuses&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;bonustext&quot;,&quot;type&quot;:&quot;bonus-texts&quot;,&quot;attributes&quot;:{&quot;text&quot;:&quot;+80 to @gabriela_buckridge @don_reinger #magni-quos-ut #non-voluptas-quia Thank you!&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1ODA4OTE1MjYsInN1YiI6NDU1LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.U4hM8PPcLQVkzPNhX24_NnJFnStyOmgq2NErky8mUjg&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{
  "data": {
    "id": "74",
    "type": "bonuses",
    "attributes": {
      "text": "+80 to @gabriela_buckridge @don_reinger #magni-quos-ut #non-voluptas-quia Thank you!",
      "points": 80,
      "total-points": 80,
      "created-at": "2020-02-04T08:32:06.801Z"
    },
    "relationships": {
      "sender": {
        "data": {
          "id": "455",
          "type": "users"
        }
      },
      "tags": {
        "data": [
          {
            "id": "543",
            "type": "tags"
          },
          {
            "id": "544",
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
            "id": "453",
            "type": "users"
          },
          {
            "id": "454",
            "type": "users"
          }
        ]
      }
    }
  },
  "included": [
    {
      "id": "455",
      "type": "users",
      "attributes": {
        "email": "hubert_jerde@schmidt.biz",
        "full-name": "Jinny Gerhold MD",
        "username": "md-jinny-gerhold",
        "profile-image-avatar-url": "memory://user/profile_image/acaac8bc7aed57a375c8b6a332b79e6f.png",
        "bonus-balance": 10000,
        "allowance-balance": 9840,
        "birth-date": "1984-11-01"
      }
    },
    {
      "id": "453",
      "type": "users",
      "attributes": {
        "email": "georgie@ernser.io",
        "full-name": "Gabriela Buckridge",
        "username": "gabriela_buckridge",
        "profile-image-avatar-url": "memory://user/profile_image/5e606aa2f4ec305fbd5ef1cf02e30ec8.png",
        "bonus-balance": 10080,
        "allowance-balance": 10000,
        "birth-date": "2019-12-09"
      }
    },
    {
      "id": "454",
      "type": "users",
      "attributes": {
        "email": "donovan@doyle.org",
        "full-name": "Don Reinger",
        "username": "don_reinger",
        "profile-image-avatar-url": "memory://user/profile_image/73e2b9391da118553e248f15a49c5451.png",
        "bonus-balance": 10080,
        "allowance-balance": 10000,
        "birth-date": "1988-03-27"
      }
    }
  ]
}</pre>
