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
    usertoken: "XXXX",
    accesstoken: "XXXX",
    userid: "XXXX"
}

const response = await fetch(`https://interact-api.novapro.net/v1/auth/checkToken`, { method: 'GET', headers })

var data = await response.json() 
```
### Returned Data
``` JSON
{
	"login": true,
	"publicData": {
		"_id": "1a03697c-5eb2-42f6-8c9b-27ed547d7493",
		"__v": 1,
		"creationTimestamp": "1697914216950",
		"description": "this account is used to test the API",
		"displayName": "dan's API",
		"followerCount": 0,
		"followingCount": 0,
		"lastEditUsername": 1697914216950,
		"likeCount": 0,
		"likedCount": 0,
		"pronouns": "he/him",
		"statusTitle": null,
		"totalPosts": 0,
		"totalReplies": 0,
		"username": "daniel_test",
		"pins": [
			{
				"_id": "671c9ad0-7230-4e6d-9301-e0160e776370",
				"timestamp": 1697914263724
			}
		]
	},
	"accessToken": "574f5e5a-bb77-47b3-a969-6ec79d0a8bf2",
	"userToken": "405ff58c-a284-455f-8667-4c0f166dd9fa",
	"userID": "1a03697c-5eb2-42f6-8c9b-27ed547d7493"
}
```