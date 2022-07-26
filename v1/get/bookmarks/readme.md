# Get User

``GET /v1/get/bookmarks``

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
| included | Object<[included](#included-object)> | 
| userData | Object<[userSchema](../../schemas/interactUserSchema.md)> |
| postData | Array<[postSchema](../../schemas/interactPostSchema.md)> |

## Included Object
| returned | type | 
| -- | -- |
| Bookmarks | Object<[postBookmarks](../../schemas/postSchemas/interactPostBookmarks.md)>

## Example of Request
### Request
Request URL

``GET https://interact-api.novapro.net/v1/get/bookmarks/``

JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX"
}

const response = await fetch(`https://interact-api.novapro.net/v1/get/bookmarks/`, { method: 'GET', headers })

var data = await response.json() 
```

### Returned Data
``` JSON
{
	"_id": "XXXX",
	"__v": 0,
	"lists": [
		{
			"_id": "62b51294ed8d0f2b6a3b0042",
			"name": "main",
			"timestamp": "1656033940628"
		}
	],
	"saves": [
		{
			"_id": "60bd41d8-bebb-42b8-b5c9-b2623b4bac17",
			"bookmarkList": "main",
			"timestamp": "1656033940628"
		},
		{
			"_id": "962d7ecc-8417-4d1b-bb96-c59816ed6ba1",
			"bookmarkList": "main",
			"timestamp": "1656033952212"
		}
	]
}
```