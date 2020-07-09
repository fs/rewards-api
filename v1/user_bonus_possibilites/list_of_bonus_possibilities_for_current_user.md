# User Bonus Possibilites API

## List of bonus possibilities for current user

### GET /api/v1/user/bonus_possibilities
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzcsInN1YiI6MzI2NCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.V69UhI5LWdqTbupnBhyfFFkHP3KHhD-fcbLTJ0fVXu4</pre>

#### Route

<pre>GET /api/v1/user/bonus_possibilities</pre>

#### Query Parameters

<pre>{}: </pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/bonus_possibilities&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzcsInN1YiI6MzI2NCwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.V69UhI5LWdqTbupnBhyfFFkHP3KHhD-fcbLTJ0fVXu4&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": {
    "id": "3264",
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
            "id": "4156",
            "type": "tags"
          }
        ]
      },
      "receivers": {
        "data": [
          {
            "id": "3263",
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
      "id": "4156",
      "type": "tags",
      "attributes": {
        "label": "ab-repellendus-possimus"
      }
    },
    {
      "id": "3263",
      "type": "users",
      "attributes": {
        "email": "sammy@littelnolan.net",
        "full-name": "Warren Raynor",
        "username": "raynor_warren",
        "profile-image-avatar-url": "memory://user/profile_image/47e9105220e66e9de2d97f1340111b11.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "2006-05-31"
      }
    }
  ]
}</pre>
