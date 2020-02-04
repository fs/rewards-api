# User Bonuses API

## List bonuses

### GET /api/v1/user/bonuses
### Request

#### Headers

<pre>Content-Type: application/vnd.api+json
Accept: application/vnd.api+json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1ODA4OTE1MjYsInN1YiI6NDQ0LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.-_MYTaWhBO1ItDbOghsu1EMqKHvwMM-NTUKIVtrvsac</pre>

#### Route

<pre>GET /api/v1/user/bonuses</pre>

#### cURL

<pre class="request">curl -g &quot;https://rewards.flts.tk/api/v1/user/bonuses&quot; -X GET \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1ODA4OTE1MjYsInN1YiI6NDQ0LCJ0eXBlIjoiYWNjZXNzIiwiY2xpZW50X2lkIjoiMiJ9.-_MYTaWhBO1ItDbOghsu1EMqKHvwMM-NTUKIVtrvsac&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{
  "data": [
    {
      "id": "69",
      "type": "bonuses",
      "attributes": {
        "text": "+61 to @stoltenberg_ellis #ut-unde-adipisci Thank you!",
        "points": 61,
        "total-points": 142,
        "created-at": "2020-02-04T08:32:06.028Z"
      },
      "relationships": {
        "sender": {
          "data": {
            "id": "442",
            "type": "users"
          }
        },
        "tags": {
          "data": [
            {
              "id": "535",
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
              "id": "443",
              "type": "users"
            }
          ]
        }
      }
    },
    {
      "id": "68",
      "type": "bonuses",
      "attributes": {
        "text": "+73 to @lilliana_brown #omnis-cupiditate-delectus Thank you!",
        "points": 73,
        "total-points": 166,
        "created-at": "2020-02-04T08:32:05.968Z"
      },
      "relationships": {
        "sender": {
          "data": {
            "id": "440",
            "type": "users"
          }
        },
        "tags": {
          "data": [
            {
              "id": "534",
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
              "id": "441",
              "type": "users"
            }
          ]
        }
      }
    }
  ],
  "included": [
    {
      "id": "442",
      "type": "users",
      "attributes": {
        "email": "odell_adams@osinski.io",
        "full-name": "Shasta Steuber",
        "username": "shasta-steuber",
        "profile-image-avatar-url": "memory://user/profile_image/8875d72f9770f518041101b949a9c3fb.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "2012-05-31"
      }
    },
    {
      "id": "535",
      "type": "tags",
      "attributes": {
        "label": "ut-unde-adipisci"
      }
    },
    {
      "id": "443",
      "type": "users",
      "attributes": {
        "email": "wiley@lebsack.net",
        "full-name": "Ellis Stoltenberg",
        "username": "stoltenberg_ellis",
        "profile-image-avatar-url": "memory://user/profile_image/2fc7f986a433d2503721c076f3cb857d.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "2015-07-30"
      }
    },
    {
      "id": "440",
      "type": "users",
      "attributes": {
        "email": "donny.torp@jerdecruickshank.net",
        "full-name": "Elinore Swaniawski",
        "username": "elinore.swaniawski",
        "profile-image-avatar-url": "memory://user/profile_image/d199eef99dcaa402ba0c973b2299f96f.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "2004-08-23"
      }
    },
    {
      "id": "534",
      "type": "tags",
      "attributes": {
        "label": "omnis-cupiditate-delectus"
      }
    },
    {
      "id": "441",
      "type": "users",
      "attributes": {
        "email": "ricky@keelingebert.co",
        "full-name": "Lilliana Brown",
        "username": "lilliana_brown",
        "profile-image-avatar-url": "memory://user/profile_image/211c4826060bc15762f531cdeb46d963.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "1980-05-09"
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
