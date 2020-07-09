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
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzcsInN1YiI6MzI2NywidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.MCoH-zuHIy2Pb4rRhfbDJhC6hhsYDaa8vLBaPjzi56o</pre>

#### Route

<pre>POST /api/v1/user/users_rewards</pre>

#### Body

<pre>{"data":{"id":"641","type":"reward-requests"}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/user/users_rewards&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;641&quot;,&quot;type&quot;:&quot;reward-requests&quot;}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzcsInN1YiI6MzI2NywidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.MCoH-zuHIy2Pb4rRhfbDJhC6hhsYDaa8vLBaPjzi56o&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{
  "data": {
    "id": "308",
    "type": "users-rewards",
    "attributes": {
      "user-id": 3267,
      "reward-id": 641,
      "created-at": "2020-07-09T08:34:37.816Z",
      "updated-at": "2020-07-09T08:34:37.816Z",
      "status": "pending",
      "purchase-price": 164,
      "company-id": 2941
    },
    "relationships": {
      "reward": {
        "data": {
          "id": "641",
          "type": "rewards"
        }
      }
    }
  },
  "included": [
    {
      "id": "641",
      "type": "rewards",
      "attributes": {
        "title": "Voluptates enim velit.",
        "price": 164,
        "created-at": "2020-07-09T08:34:37.678Z",
        "updated-at": "2020-07-09T08:34:37.678Z",
        "url": "http://ebert.org/willy.green",
        "image-data": "{\"id\":\"reward/image/ce32f57a081581161aeb41662b201187.png\",\"storage\":\"cache\",\"metadata\":{\"filename\":\"reward-image.png\",\"size\":3011,\"mime_type\":\"image/png\"}}",
        "company-id": 2941,
        "unlimited": true,
        "available-amount": 57,
        "archived": false,
        "type": "Reward"
      }
    }
  ]
}</pre>
