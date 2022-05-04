# get post

``GET /v1/get/post/:postid``

[Example of Request](#example-of-request)

## Required 
| location | required | type | optional |
| -- | -- | -- | -- |
| url param | postid | String | false |
| header | devtoken | String | false |
| header | apptoken | String | false |
| header | accesstoken | String | false |
| header | usertoken | String | false |
| header | userid | String | false |

## Returned Data
| returned | type | 
| -- | -- |
| Post Object | Object<[postSchema](../../schemas/interactPostSchema.md)> |

## Example of Request
### Request
Request URL

``GET https://interact-api.novapro.net/v1/get/post/:postid``

JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX"
}

const response = await fetch(`https://interact-api.novapro.net/v1/get/post/790919b8-c095-4c81-a515-ec8f8eb72145`, { method: 'GET', headers })

var data = await response.json() 
```

### Returned Data
``` JSON
{
	"_id": "790919b8-c095-4c81-a515-ec8f8eb72145",
	"__v": 1,
	"content": "I keep forgetting which user im using, so im using this as a check to see my userID",
	"timePosted": "1647282601269",
	"totalLikes": 0,
	"totalReplies": 0,
	"userID": "6ceae342-2ca2-48ec-8ce3-0e39caebe989"
}
```