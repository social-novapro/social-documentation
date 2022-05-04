# search

``GET /v1/get/search/``

[Example of Request](#example-of-request)

## Required 
| location | required | type | optional |
| -- | -- | -- | -- |
| header | lookupkey | String | false |
| header | devtoken | String | false |
| header | apptoken | String | false |
| header | accesstoken | String | false |
| header | usertoken | String | false |
| header | userid | String | false |

## Returned Data
| returned | type | 
| -- | -- |
| usersFound | Array<[userSchema](../../schemas/interactUserSchema.md)> |
| postsFound | Array<[postSchema](../../schemas/interactPostSchema.md)> |

## Example of Request
### Request
Request URL

``GET https://interact-api.novapro.net/v1/get/search``

JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX",
    lookupkey: "daniel"
}

const response = await fetch(`https://interact-api.novapro.net/v1/get/search`, { method: 'GET', headers})

var data = await response.json() 
```

### Returned Data
``` JSON
{
	"usersFound": [
		{
			"_id": "68644de9-8694-4268-ad08-61a1dcb6c6c5",
			"__v": 1,
			"creationTimestamp": "1627404095483",
			"followerCount": 0,
			"followingCount": 0,
			"likeCount": 0,
			"likedCount": 0,
			"totalPosts": 0,
			"totalReplies": 0,
			"displayName": "Daniel Kravec",
			"username": "dkravec"
		},
        {
			"_id": "32751e8e-0b7f-42e3-9ab7-b38dd53c0da8",
			"__v": 1,
			"creationTimestamp": "1651073052986",
			"description": "Hello, its me Daniel! The Creator of Interact!",
			"displayName": "Daniel Kravec",
			"followerCount": 0,
			"followingCount": 0,
			"lastEditDisplayname": 1651073052986,
			"lastEditUsername": 1651073052986,
			"likeCount": 0,
			"likedCount": 0,
			"pronouns": null,
			"statusTitle": null,
			"totalPosts": 0,
			"totalReplies": 0,
			"username": "thisTeste"
		}
    ],
    "postsFound": [
		{
			"type": {
				"type": "post",
				"user": "included"
			},
			"postData": {
				"_id": "117892f9-e035-404a-9e23-a3da5772041a",
				"__v": 1,
				"content": "daniel kravec is my name",
				"timePosted": "1630205636767",
				"totalLikes": 0,
				"totalReplies": 0,
				"userID": "d825813d-95d2-46eb-868a-ae2e850eab92"
			},
			"userData": {
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
		}
	]
}
```