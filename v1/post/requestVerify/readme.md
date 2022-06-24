# Request verification

``GET /v1/post/requestVerify``

[Example of Request](#example-of-request)

## Required 
| location | required | type | optional |
| -- | -- | -- | -- |
| body | content | String | false |
| header | devtoken | String | false |
| header | apptoken | String | false |
| header | accesstoken | String | false |
| header | usertoken | String | false |
| header | userid | String | false |

## Returned Data
| returned | type | 
| -- | -- |
| Object | Object<{\_id, \_\_v, timestamp, content}> |

## Example of Request
### Request
Request URL

``POST https://interact-api.novapro.net/v1/post/requestVerify``

JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX"
}
const data = {
    content: "XXXX"
}
const response = await fetch(`https://interact-api.novapro.net/v1/post/requestVerify`, { 
    method: 'POST', 
    headers, 
    body: JSON.Stringify(data) 
})

var data = await response.json() 
```

### Returned Data
``` JSON
{
	"_id": "60628cba-a55e-43cd-83e8-3da4c44c104f",
	"__v": 1,
	"content": "XXXX",
	"timestamp": "1655067676910",
}
```
