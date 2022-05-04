# Get User

``GET /v1/get/user/:userid``

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
| included | Object<[included](#included-object)> | 
| userData | Object<[userSchema](../../schemas/interactUserSchema.md)> |
| postData | Array<[postSchema](../../schemas/interactPostSchema.md)> |

## Included Object
| returned | type | 
| -- | -- |
| users | String (should be Boolean) | 
| posts | String (should be Boolean) | 

## Example of Request
### Request
Request URL

``GET https://interact-api.novapro.net/v1/get/user/:userid``

JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX"
}

const response = await fetch(`https://interact-api.novapro.net/v1/get/user/6ceae342-2ca2-48ec-8ce3-0e39caebe989`, { method: 'GET', headers })

var data = await response.json() 
```

### Returned Data
``` JSON
{
	"included": {
		"user": "true",
		"posts": "true"
	},
	"userData": {
		"_id": "6ceae342-2ca2-48ec-8ce3-0e39caebe989",
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
	"postData": [
		{
			"_id": "41ef1a02-66ee-437b-9334-193c3472c56d",
			"__v": 1,
			"content": "this is a test",
			"timePosted": "1647275392271",
			"totalLikes": 0,
			"totalReplies": 0,
			"userID": "6ceae342-2ca2-48ec-8ce3-0e39caebe989"
		},
		{
			"_id": "e3244f07-6a86-4b02-aaef-7176b24549b1",
			"__v": 1,
			"content": "after requiring shit",
			"timePosted": "1647275759707",
			"totalLikes": 0,
			"totalReplies": 0,
			"userID": "6ceae342-2ca2-48ec-8ce3-0e39caebe989"
		},
		{
			"_id": "790919b8-c095-4c81-a515-ec8f8eb72145",
			"__v": 1,
			"content": "I keep forgetting which user im using, so im using this as a check to see my userID",
			"timePosted": "1647282601269",
			"totalLikes": 17,
			"totalReplies": 0,
			"userID": "6ceae342-2ca2-48ec-8ce3-0e39caebe989"
		},
		{
			"_id": "81210231-0343-4838-8a34-38d72cee19e0",
			"__v": 1,
			"content": "test",
			"timePosted": "1648661741403",
			"totalLikes": 0,
			"totalReplies": 0,
			"userID": "6ceae342-2ca2-48ec-8ce3-0e39caebe989"
		},
    ]
}
```