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
| header | newUsername | String | true* |
| header | newDisplayname | String | true* |
| header | newPronouns | String | true* |
| header | newDescription | String | true* |
| header | newStatus | String | true* |

**the amount of optional headers must be between 1 and 5 inclusive*

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
    method: 'PUT',
    headers,
});

// you must convert the data from a string to json
var res = await response.json()
```

### Returned Data
``` JSON
{
  "new": {
    "_id": "XXXX",
    "__v": 1,
    "creationTimestamp": "1648174890907",
    "description": "XXXX",
    "displayName": "YYYY",
    "followerCount": 0,
    "followingCount": 0,
    "lastEditDisplayname": 1656208206255,
    "lastEditUsername": 1648174890907,
    "likeCount": 0,
    "likedCount": 0,
    "pronouns": "ABC/DEF",
    "statusTitle": null,
    "totalPosts": 0,
    "totalReplies": 0,
    "username": "XXXX"
  },
  "before": {
    "_id": "XXXX",
    "__v": 1,
    "creationTimestamp": "1648174890907",
    "description": "XXXX",
    "displayName": "XXXX",
    "followerCount": 0,
    "followingCount": 0,
    "lastEditDisplayname": 1656074181261,
    "lastEditUsername": 1648174890907,
    "likeCount": 0,
    "likedCount": 0,
    "pronouns": "GHI/JKL",
    "statusTitle": null,
    "totalPosts": 0,
    "totalReplies": 0,
    "username": "XXXX"
  }
}
```