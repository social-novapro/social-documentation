# userEdit

``PUT /v1/put/userEdit/``

[Example of Request](#example-of-request)

## Required
| location | required | type | optional |
| -- | -- | -- | -- |
| header | devtoken | String | false |
| header | apptoken | String | false |
| header | accesstoken | String | false |
| header | usertoken | String | false |
| header | userid | String | false |
| -- | at least one of below | -- | -- |
| header | newUsername | String | true | 
| header | newDisplayname | String | true | 
| header | newDescription | String | true | 
| header | newPronouns | String | true | 
| header | newStatus | String | true | 

## Returned Data
| returned | type | 
| -- | -- |
| new | Object<[userSchema](../../schemas/interactUserSchema.md)> |
| before | Object<[userSchema](../../schemas/interactUserSchema.md)> |


## Example of Request
### Request
Request URL

``https://interact-api.novapro.net/v1/put/userEdit``

### JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX",
    newUsername: "XXXX", // Optional Requires At Least One
    newDisplayname: "XXXX", // Optional Requires At Least One
    newDescription: "XXXX", // Optional Requires At Least One
    newPronouns: "XXXX", // Optional Requires At Least One
    newStatus: "XXXX", // Optional Requires At Least One
}

const response = await fetch(`https://interact-api.novapro.net/v1/put/userEdit`, {
    method: 'POST',
    headers
});

// you must convert the data from a string to json
var res = await response.json()
```

### Returned Data
``` JSON
{
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
    "username": "dan2364755",
    "lastEdit": 1646367628998
}
```