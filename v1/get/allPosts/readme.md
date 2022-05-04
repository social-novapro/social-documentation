# allPosts

``GET /v1/get/allPosts/``

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
| Array | Array<[Object](#arrayeach)> |


### arrayEach
| Field | Type | Optional | Description |
| -- | -- | -- | -- |
| type | Object<[type](#type-object)> | false | This includes the informatino for the rest of current Object. |
| postData | Object<[postSchema](../../schemas/interactUserSchema.md)> | false | This includes data of the found post.
| userData | Object<[userSchema](../../schemas/interactUserSchema.md)> | true | This includes the data of the user who posted the found post.

### type object
| Field | Type | Optional | Description |
| -- | -- | -- | -- |
| type | String | false | What is the returned type of data. String will be "post". |
| user | String | true | Is there a user included in the main object. String will be "included" if there is any. |


## Example of Request
### Request
Request URL

``GET https://interact-api.novapro.net/v1/get/allPosts``

JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX"
}

const response = await fetch(`https://interact-api.novapro.net/v1/get/allPosts`, { method: 'GET', headers})

var data = await response.json() 
```

### Returned Data
``` JSON
[
    {
		"type": {
			"type": "post"
		},
		"postData": {
			"_id": "5a74e7e2-82af-4e75-ba0b-4af549d2c27e",
			"__v": 1,
			"timePosted": "1627402703406",
			"totalLikes": 0,
			"totalReplies": 0,
			"content": "Hello my name is daniel, this is a test post!",
			"userID": "0001"
		}
	},
    {
		"type": {
			"type": "post",
			"user": "included"
		},
		"postData": {
			"_id": "482e2ee4-ce99-465c-aefa-8931f5c16708",
			"__v": 1,
			"timePosted": "1627782452149",
			"totalLikes": 0,
			"totalReplies": 0,
			"content": "This is a test"
		},
		"userData": {
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
		}
	},
    {
		"type": {
			"type": "post",
			"user": "included"
		},
		"postData": {
			"_id": "83734077-7a3b-4eaf-b2b9-cb8efdc2f5f8",
			"__v": 1,
			"content": "testing posting from frontend! not first",
			"timePosted": "1630671911201",
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
```