# Users Rewards API

## Create reward request

### POST /api/v1/user/users_rewards

### Parameters

| Name | Description | Required | Scope |
|------|-------------|----------|-------|
| id |  id | false |  |

### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjgwNzY4MDUsInN1YiI6MjM0MiwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.Wz1vqWBdOrF-Enqn-BhtPTBumjZ9OZ55VFpzcIgbr1U</pre>

#### Route

<pre>POST /api/v1/user/users_rewards</pre>

#### Body

<pre>{"data":{"id":"267","type":"reward-requests"}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/user/users_rewards&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;267&quot;,&quot;type&quot;:&quot;reward-requests&quot;}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjgwNzY4MDUsInN1YiI6MjM0MiwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.Wz1vqWBdOrF-Enqn-BhtPTBumjZ9OZ55VFpzcIgbr1U&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{
  "data": {
    "id": "140",
    "type": "users-rewards",
    "attributes": {
      "user-id": 2342,
      "reward-id": 267,
      "created-at": "2021-08-03T11:33:25.869Z",
      "updated-at": "2021-08-03T11:33:25.869Z",
      "status": "pending",
      "purchase-price": 391,
      "company-id": 2012
    },
    "relationships": {
      "reward": {
        "data": {
          "id": "267",
          "type": "rewards"
        }
      }
    }
  },
  "included": [
    {
      "id": "267",
      "type": "rewards",
      "attributes": {
        "title": "Odio et ut.",
        "price": 391,
        "created-at": "2021-08-03T11:33:25.802Z",
        "updated-at": "2021-08-03T11:33:25.802Z",
        "url": "http://beattyreilly.name/tad",
        "image-data": "{\"id\":\"reward/image/d077c84e2e5fc85c1ab28d4a317109f4.png\",\"storage\":\"cache\",\"metadata\":{\"filename\":\"reward-image.png\",\"size\":3011,\"mime_type\":\"image/png\"}}",
        "company-id": 2012,
        "unlimited": true,
        "available-amount": 35,
        "archived": false
      }
    }
  ]
}</pre>
