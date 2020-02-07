# User Bonus Possibilites API

## List of bonus possibilities for current user

### GET /api/v1/user/bonus_possibilities
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1ODA4OTE1MjMsInN1YiI6NDE4LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.8ga_dw0q9CepPHLOMYZRyiM8Iir0OWYFWtJGts614CY</pre>

#### Route

<pre>GET /api/v1/user/bonus_possibilities</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.flts.tk/api/v1/user/bonus_possibilities&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1ODA4OTE1MjMsInN1YiI6NDE4LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.8ga_dw0q9CepPHLOMYZRyiM8Iir0OWYFWtJGts614CY&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": {
    "id": "418",
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
            "id": "509",
            "type": "tags"
          }
        ]
      },
      "receivers": {
        "data": [
          {
            "id": "417",
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
      "id": "509",
      "type": "tags",
      "attributes": {
        "label": "vitae-aut-quos"
      }
    },
    {
      "id": "417",
      "type": "users",
      "attributes": {
        "email": "malik@lang.net",
        "full-name": "Kindra Yundt",
        "username": "kindra-yundt",
        "profile-image-avatar-url": "memory://user/profile_image/e44f0ca6e4a1a9c85833c90dff242590.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "2013-05-13"
      }
    }
  ]
}</pre>
