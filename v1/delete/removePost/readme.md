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
| post* | Object<[postSchema](../../schemas/interactPostSchema.md)> |

\**only in newer api version*

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
    "deleted" : "true",
    "post" : {
        "__v": 1,
        "_id": "1521ef6b-e768-4ea7-867d-bfe0c20c71b2",
        "content": "test",
        "timePosted": "1651081504275",
        "totalLikes": 0,
        "totalReplies": 0,
        "userID": "32751e8e-0b7f-42e3-9ab7-b38dd53c0da8"
    }
}
```