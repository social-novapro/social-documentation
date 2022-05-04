# Get User by Username

``GET /v1/get/username/:username``

[Example of Request](#example-of-request)

## Required 
| location | required | type | optional |
| -- | -- | -- | -- |
| url param | username | String | false | 
| header | devtoken | String | false |
| header | apptoken | String | false |
| header | accesstoken | String | false |
| header | usertoken | String | false |
| header | userid | String | false |

## Returned Data
| returned | type | 
| -- | -- |
| user | Object<[userSchema](../../schemas/interactUserSchema.md)> |

## Example of Request
### Request
Request URL

``GET https://interact-api.novapro.net/v1/get/username/:username``

JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX" ,
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX"
}

const response = await fetch(`https://interact-api.novapro.net/v1/get/username/dan`, { method: 'GET', headers })

var data = await response.json() 
```

### Returned Data
``` JSON
{
	"_id": "11bc2227-ba91-4973-b633-e294b37a1a30",
	"__v": 1,
	"creationTimestamp": "1627901461543",
	"displayName": "Daniel Kravec Again",
	"followerCount": 0,
	"followingCount": 0,
	"likeCount": 0,
	"likedCount": 0,
	"totalPosts": 0,
	"totalReplies": 0,
	"username": "dan"
}
```