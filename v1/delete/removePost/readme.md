# removePost

``DELETE /v1/delete/removePost/:postID``
| location | required | type | optional |
| -- | -- | -- | -- |
| url param | postID | String | false
| header | devtoken | String | false |
| header | apptoken | String | false |
| header | accesstoken | String | false |
| header | usertoken | String | false |
| header | userid | String | false |

| returned | type | 
| -- | -- |
| deleted | Boolean |


## Example of Request
### Request
Request URL

``GET https://interact-api.novapro.net/v1/delete/removePost/:postID``

### JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX"
}

const response = await fetch(`https://interact-api.novapro.net/v1/delete/removePost/XXXX`, { 
    method: 'DELETE', 
    headers
})

var data = await response.json() 
```

### Returned Data
``` JSON
{
    "deleted" : "true"
}
```