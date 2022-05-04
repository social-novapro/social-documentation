# allPosts

``GET /v1/get/allUsers/``

[Example of Request](#example-of-request)

## Required 
| location | required | type | optional |
| -- | -- | -- | -- |
| header | devtoken | String | false |
| header | apptoken | String | false |
| header | accesstoken | String | false |
| header | usertoken | String | false |
| header | userid | String | false |

## Returned Data
| returned | type | 
| -- | -- |
| Array | Array<[interactUserSchema](../../schemas/interactUserSchema.md)> |

## Example of Request
### Request
Request URL

``GET https://interact-api.novapro.net/v1/get/allUsers``

JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX"
}

const response = await fetch(`https://interact-api.novapro.net/v1/get/allUsers`, { method: 'GET', headers})

var data = await response.json() 
```

### Returned Data
``` JSON
[
    {
        "_id": "5c210553-dc0d-4cdd-82fc-75b4f8974841",
        "__v": 1,
        "creationTimestamp": "1627776147223",
        "displayName": "Daniel Kravec",
        "followerCount": 0,
        "followingCount": 0,
        "likeCount": 0,
        "likedCount": 0,
        "totalPosts": 0,
        "totalReplies": 0,
        "username": "danny101"
    }, 
    {
        "_id": "d825813d-95d2-46eb-868a-ae2e850eab92",
        "__v": 1,
        "creationTimestamp": "1627930355803",
        "displayName": "Daniel Tester",
        "followerCount": 0,
        "followingCount": 0,
        "lastEditUsername": 1630616479209,
        "likeCount": 0,
        "likedCount": 0,
        "totalPosts": 0,
        "totalReplies": 0,
        "username": "editUsernameFrontend",
        "lastEditDisplayname": 1628035524271
    }
]
```