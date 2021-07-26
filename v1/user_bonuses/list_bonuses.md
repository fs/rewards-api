# User Bonuses API

## List bonuses

### GET /api/v1/user/bonuses
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzMsInN1YiI6MTk2MiwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.CLy42H0eiISkDbPWAZZMpf-vVBWKBJpdKizfZbvTn-E</pre>

#### Route

<pre>GET /api/v1/user/bonuses</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.team/api/v1/user/bonuses&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjczNzg1MzMsInN1YiI6MTk2MiwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.CLy42H0eiISkDbPWAZZMpf-vVBWKBJpdKizfZbvTn-E&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": [
    {
      "id": "309",
      "type": "bonuses",
      "attributes": {
        "text": "+13 to @simonis-dominick-miss #facere-quis-molestiae Thank you!",
        "points": 13,
        "total-points": 69,
        "created-at": "2021-07-26T09:35:33.597Z"
      },
      "relationships": {
        "sender": {
          "data": {
            "id": "1960",
            "type": "users"
          }
        },
        "tags": {
          "data": [
            {
              "id": "2399",
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
              "id": "1961",
              "type": "users"
            }
          ]
        }
      }
    },
    {
      "id": "308",
      "type": "bonuses",
      "attributes": {
        "text": "+73 to @rodriguez-crysta #voluptatem-sapiente-aut Thank you!",
        "points": 73,
        "total-points": 147,
        "created-at": "2021-07-26T09:35:33.532Z"
      },
      "relationships": {
        "sender": {
          "data": {
            "id": "1958",
            "type": "users"
          }
        },
        "tags": {
          "data": [
            {
              "id": "2398",
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
              "id": "1959",
              "type": "users"
            }
          ]
        }
      }
    }
  ],
  "included": [
    {
      "id": "1960",
      "type": "users",
      "attributes": {
        "email": "berry@adamsabernathy.biz",
        "full-name": "Dr. Adolph Russel",
        "username": "russel.adolph.dr",
        "profile-image-avatar-url": "memory://user/profile_image/47a8905611b990c416302751c76a8fd6.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "2010-05-05"
      }
    },
    {
      "id": "2399",
      "type": "tags",
      "attributes": {
        "label": "facere-quis-molestiae"
      }
    },
    {
      "id": "1961",
      "type": "users",
      "attributes": {
        "email": "susie.kautzer@bailey.io",
        "full-name": "Miss Dominick Simonis",
        "username": "simonis-dominick-miss",
        "profile-image-avatar-url": "memory://user/profile_image/669d8185110a420cef22288515bcd9ab.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "1985-06-13"
      }
    },
    {
      "id": "1958",
      "type": "users",
      "attributes": {
        "email": "tamiko@beckerboyer.io",
        "full-name": "Prince Bayer",
        "username": "bayer.prince",
        "profile-image-avatar-url": "memory://user/profile_image/f5b584c47d32f998787d4725a272ffe6.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "1986-05-26"
      }
    },
    {
      "id": "2398",
      "type": "tags",
      "attributes": {
        "label": "voluptatem-sapiente-aut"
      }
    },
    {
      "id": "1959",
      "type": "users",
      "attributes": {
        "email": "jammie.rowe@grahamhintz.info",
        "full-name": "Crysta Rodriguez",
        "username": "rodriguez-crysta",
        "profile-image-avatar-url": "memory://user/profile_image/5163cdedf59de44d55675e5d0e2b2f90.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "1997-04-18"
      }
    }
  ],
  "links": {
    "self": "http://example.org/api/v1/user/bonuses?page%5Bnumber%5D=1&page%5Bsize%5D=10",
    "first": "http://example.org/api/v1/user/bonuses?page%5Bnumber%5D=1&page%5Bsize%5D=10",
    "prev": null,
    "next": null,
    "last": "http://example.org/api/v1/user/bonuses?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  }
}</pre>
