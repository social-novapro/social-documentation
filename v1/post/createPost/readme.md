# createPost

``POST /v1/post/createPost/``

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
| deleted | Boolean |


## Example of Request
### Request
Request URL

``https://interact-api.novapro.net/v1/post/createPost``

### JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX"
}

const data = { 
    "userID" : "XXXX", 
    "content" : "input",
    "quoteReplyPostID" : "XXXX"
};

const response = await fetch(`https://interact-api.novapro.net/v1/post/createPost`, {
    method: 'POST',
    headers,
    body: JSON.stringify(data)
});

// you must convert the data from a string to json
var res = await response.json()
```

### Returned Data
``` JSON
{
    "__v": 1,
    "_id": "1521ef6b-e768-4ea7-867d-bfe0c20c71b2",
    "content": "test",
    "timePosted": "1651081504275",
    "totalLikes": 0,
    "totalReplies": 0,
    "userID": "32751e8e-0b7f-42e3-9ab7-b38dd53c0da8"
}
```