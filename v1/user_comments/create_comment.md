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
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzgsInN1YiI6MzI3MiwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.KscqFTUYYSumYHM-tqogS87WHnxaNqTpP14S3NmgfHc</pre>

#### Route

<pre>POST /api/v1/user/bonuses/633/comments</pre>

#### Body

<pre>{"data":{"id":"commenttext","type":"comment-texts","attributes":{"text":"+66 Eos qui est unde. #eos-ad-ipsum #dolor-dolores-iure"}}}</pre>

#### cURL

<pre class="request">curl &quot;https://rewards.team/api/v1/user/bonuses/633/comments&quot; -d &#39;{&quot;data&quot;:{&quot;id&quot;:&quot;commenttext&quot;,&quot;type&quot;:&quot;comment-texts&quot;,&quot;attributes&quot;:{&quot;text&quot;:&quot;+66 Eos qui est unde. #eos-ad-ipsum #dolor-dolores-iure&quot;}}}&#39; -X POST \
	-H &quot;Content-Type: application/vnd.api+json&quot; \
	-H &quot;Accept: application/vnd.api+json&quot; \
	-H &quot;Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE1OTQzNzAwNzgsInN1YiI6MzI3MiwidHlwZSI6ImFjY2VzcyIsImNsaWVudF9pZCI6IjIifQ.KscqFTUYYSumYHM-tqogS87WHnxaNqTpP14S3NmgfHc&quot;</pre>

### Response

#### Headers

<pre>Content-Type: application/vnd.api+json; charset=utf-8</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{
  "data": {
    "id": "633",
    "type": "bonuses",
    "attributes": {
      "text": "+29 to @carolynn-mcclure #laboriosam-veniam-nobis Thank you!",
      "points": 29,
      "total-points": 176,
      "created-at": "2020-07-09T08:34:38.306Z"
    },
    "relationships": {
      "sender": {
        "data": {
          "id": "3270",
          "type": "users"
        }
      },
      "tags": {
        "data": [
          {
            "id": "4165",
            "type": "tags"
          }
        ]
      },
      "comments": {
        "data": [
          {
            "id": "49",
            "type": "comments"
          }
        ]
      },
      "receivers": {
        "data": [
          {
            "id": "3271",
            "type": "users"
          }
        ]
      }
    }
  },
  "included": [
    {
      "id": "3270",
      "type": "users",
      "attributes": {
        "email": "hilario@stokes.info",
        "full-name": "Sheryll O'Hara",
        "username": "sheryll.hara.o",
        "profile-image-avatar-url": "memory://user/profile_image/9d997f8113692f5aa6f35b60e453c68e.png",
        "bonus-balance": 10000,
        "allowance-balance": 10000,
        "birth-date": "1971-10-07"
      }
    },
    {
      "id": "49",
      "type": "comments",
      "attributes": {
        "created-at": "2020-07-09T08:34:38.435Z",
        "text": "+66 Eos qui est unde. #eos-ad-ipsum #dolor-dolores-iure"
      },
      "relationships": {
        "bonus": {
          "data": {
            "id": "633",
            "type": "bonuses"
          }
        },
        "sender": {
          "data": {
            "id": "3272",
            "type": "users"
          }
        },
        "tags": {
          "data": []
        }
      }
    },
    {
      "id": "3272",
      "type": "users",
      "attributes": {
        "email": "herschel@king.co",
        "full-name": "Dr. Jacque Spencer",
        "username": "jacque_spencer_dr",
        "profile-image-avatar-url": "memory://user/profile_image/b48ec22454a646c853e6d0c4a1e25832.png",
        "bonus-balance": 10000,
        "allowance-balance": 9934,
        "birth-date": "2016-03-16"
      }
    },
    {
      "id": "3271",
      "type": "users",
      "attributes": {
        "email": "gale_johns@champlinvandervort.org",
        "full-name": "Carolynn McClure",
        "username": "carolynn-mcclure",
        "profile-image-avatar-url": "memory://user/profile_image/8ff369a1196dbab233e22063df4f461d.png",
        "bonus-balance": 10066,
        "allowance-balance": 10000,
        "birth-date": "1985-05-06"
      }
    }
  ]
}</pre>
