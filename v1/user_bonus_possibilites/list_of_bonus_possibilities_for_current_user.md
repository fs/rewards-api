# User Bonus Possibilites API

## List of bonus possibilities for current user

### GET /api/v1/user/bonus_possibilities
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzUsInN1YiI6MTk4MCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.jII_ElygFvfd3fVR1CO8IO58PcLQBJ0UdMgmNjIhGyI</pre>

#### Route

<pre>GET /api/v1/user/bonus_possibilities</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/bonus_possibilities&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzUsInN1YiI6MTk4MCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.jII_ElygFvfd3fVR1CO8IO58PcLQBJ0UdMgmNjIhGyI&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": {
    "id": "1980",
    "type": "bonus-possibilities",
    "relationships": {
      "amounts": {
        "data": [
          {
            "id": "50",
            "type": "points"
          },
          {
            "id": "250",
            "type": "points"
          },
          {
            "id": "500",
            "type": "points"
          },
          {
            "id": "750",
            "type": "points"
          },
          {
            "id": "1000",
            "type": "points"
          },
          {
            "id": "1250",
            "type": "points"
          }
        ]
      },
      "tags": {
        "data": [
          {
            "id": "2418",
            "type": "tags"
          }
        ]
      },
      "receivers": {
        "data": [
          {
            "id": "1979",
            "type": "users"
          }
        ]
      }
    }
  },
  "included": [
    {
      "id": "50",
      "type": "points",
      "attributes": {
        "value": 50
      }
    },
    {
      "id": "250",
      "type": "points",
      "attributes": {
        "value": 250
      }
    },
    {
      "id": "500",
      "type": "points",
      "attributes": {
        "value": 500
      }
    },
    {
      "id": "750",
      "type": "points",
      "attributes": {
        "value": 750
      }
    },
    {
      "id": "1000",
      "type": "points",
      "attributes": {
        "value": 1000
      }
    },
    {
      "id": "1250",
      "type": "points",
      "attributes": {
        "value": 1250
      }
    },
    {
      "id": "2418",
      "type": "tags",
      "attributes": {
        "label": "officia-debitis-ut"
      }
    },
    {
      "id": "1979",
      "type": "users",
      "attributes": {
        "email": "cathy.swift@stammrau.co",
        "full-name": "Harvey Witting III",
        "username": "witting.iii.harvey",
        "profile-image-avatar-url": "memory://user/profile_image/ccd08732d22584c7e727ac2fbec62637.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "2011-06-22"
      }
    }
  ]
}</pre>
