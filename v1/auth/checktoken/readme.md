# checkToken

``GET /v1/auth/checkToken/``

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
| accessToken | String |
| userToken | String |
| userID | String |
| publicData | [publicData](../../schemas/interactUserSchema.md) | 
| login | Boolean | 


## Example of Request
### Request
Request URL

``GET https://interact-api.novapro.net/v1/auth/checkToken``
### JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    username: "XXXX",
    password: "XXXX"
}

const response = await fetch(`https://interact-api.novapro.net/v1/auth/checkToken`, { method: 'GET', headers})

var data = await response.json() 
```
### Returned Data
``` JSON
{
	"login": true,
	"publicData": {
		"_id": "XXXX", // userid
		"__v": 1,
		"creationTimestamp": "1646367628998",
		"description": "Hello, its me Daniel! The Creator of Interact!",
		"displayName": "Daniel Kravec",
		"followerCount": 0,
		"followingCount": 0,
		"lastEditDisplayname": 1646367628998,
		"lastEditUsername": 1646367628998,
		"likeCount": 0,
		"likedCount": 0,
		"pronouns": null,
		"statusTitle": null,
		"totalPosts": 0,
		"totalReplies": 0,
		"username": "dan2364755"
	},
	"accessToken": "XXXX",
	"userToken": "XXXX",
	"userID": "XXXX"
}
```