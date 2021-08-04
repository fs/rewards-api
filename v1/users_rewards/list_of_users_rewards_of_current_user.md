# Users Rewards API

## List of users_rewards of current user

### GET /api/v1/user/users_rewards
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjgwNzY4MDUsInN1YiI6MjMzOSwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.CXQwSQtYr5afEpP4J-YVvNQIJzWCuJOcVuLlz1MzO3k</pre>

#### Route

<pre>GET /api/v1/user/users_rewards</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/users_rewards&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjgwNzY4MDUsInN1YiI6MjMzOSwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.CXQwSQtYr5afEpP4J-YVvNQIJzWCuJOcVuLlz1MzO3k&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": [
    {
      "id": "137",
      "type": "users-rewards",
      "attributes": {
        "user-id": 2339,
        "reward-id": 264,
        "created-at": "2021-08-03T11:33:25.253Z",
        "updated-at": "2021-08-03T11:33:25.253Z",
        "status": "pending",
        "purchase-price": 287,
        "company-id": 2007
      },
      "relationships": {
        "reward": {
          "data": {
            "id": "264",
            "type": "rewards"
          }
        }
      }
    }
  ],
  "included": [
    {
      "id": "264",
      "type": "rewards",
      "attributes": {
        "title": "Omnis accusamus rerum.",
        "price": 287,
        "created-at": "2021-08-03T11:33:25.249Z",
        "updated-at": "2021-08-03T11:33:25.249Z",
        "url": "http://dubuquejones.org/shirley.harvey",
        "image-data": "{\"id\":\"reward/image/eeab3c5e1fb511650b5ec9b58866d4fc.png\",\"storage\":\"cache\",\"metadata\":{\"filename\":\"reward-image.png\",\"size\":3011,\"mime_type\":\"image/png\"}}",
        "company-id": 2007,
        "unlimited": true,
        "available-amount": 5,
        "archived": false
      }
    }
  ]
}</pre>
