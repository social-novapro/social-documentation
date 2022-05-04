# createPost

``GET /v1/get/allPublicData/``
| location | required | type | optional |
| -- | -- | -- | -- |
| header | devtoken | String | false |
| header | apptoken | String | false |
| header | accesstoken | String | false |
| header | usertoken | String | false |
| header | userid | String | false |

| returned | type | 
| -- | -- |
| posts | Array<[postSchema](../../schemas/interactPostSchema.md)> |
| users | Array<[userSchema](../../schemas/interactUserSchema.md)> |


## Example of Request
### Request
Request URL

``https://interact-api.novapro.net/v1/get/allPublicData``

### JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX"
}

const response = await fetch(`https://interact-api.novapro.net/v1/get/allPublicData`, { 
    method: 'GET', 
    headers,
});

var res = await response.json()
```

### Returned Data
``` JSON
{
    "posts" : [
        {
			"_id": "22186991-4222-437f-9c7e-bd2921e67fac",
			"__v": 1,
			"content": "rqkuhlirq",
			"timePosted": "1643204934532",
			"totalLikes": 0,
			"totalReplies": 0,
			"userID": "95ac47d8-5afb-4083-98aa-de6dec4df754"
		},
        {
			"_id": "476062b5-9a98-4d04-836e-3497d52de8ce",
			"__v": 1,
			"content": "does quoting work yet",
			"timePosted": "1648705589913",
			"totalLikes": 0,
			"totalReplies": 0,
			"userID": "d2ac792f-0f5a-443d-8453-f8396e1b6303",
			"quoteReplyPostID": "cc12914f-25a1-4191-89a6-38993943893e",
			"quotedPost": {
				"_id": "cc12914f-25a1-4191-89a6-38993943893e",
				"content": "...",
				"timePosted": "1648705544875",
				"totalLikes": 0,
				"totalReplies": 0,
				"userID": "d2ac792f-0f5a-443d-8453-f8396e1b6303"
			},
			"quotedUser": {
				"_id": "d2ac792f-0f5a-443d-8453-f8396e1b6303",
				"creationTimestamp": "1647915123292",
				"description": "danTest is new to Interact, make sure to say hello!",
				"displayName": "daneafaoj",
				"followerCount": 0,
				"followingCount": 0,
				"lastEditDisplayname": 1647915123292,
				"lastEditUsername": 1647915123292,
				"likeCount": 0,
				"likedCount": 0,
				"pronouns": null,
				"statusTitle": null,
				"totalPosts": 0,
				"totalReplies": 0,
				"username": "danTest"
			}
		},
    ],
    "users" : [
        {
			"_id": "5cd66ec9-5c2c-403e-8dde-b8a28b67f796",
			"__v": 1,
			"creationTimestamp": "1648426901509",
			"description": "nojnpjnop",
			"displayName": " jinionon",
			"followerCount": 0,
			"followingCount": 0,
			"lastEditDisplayname": 1648426901509,
			"lastEditUsername": 1648426901509,
			"likeCount": 0,
			"likedCount": 0,
			"pronouns": "nojpnpon ",
			"statusTitle": null,
			"totalPosts": 0,
			"totalReplies": 0,
			"username": "testing101"
		},
        {
			"_id": "036bd51e-0cfa-4c46-85fc-9d37e1514652",
			"__v": 1,
			"creationTimestamp": "1627900944176",
			"displayName": "Daniel Kravec Again",
			"followerCount": 0,
			"followingCount": 0,
			"likeCount": 0,
			"likedCount": 0,
			"totalPosts": 0,
			"totalReplies": 0,
			"username": "daniel"
		},
    ]
}
```