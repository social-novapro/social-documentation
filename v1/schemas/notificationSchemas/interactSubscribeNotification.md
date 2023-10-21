# interactSubscribeNotification
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID (of person who posts) |
| subscribed | [userSub[]](#usersub) | false | array of userSub |

## userSub
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID (of person who subbed) |
| timestamp | number | true | time subscribed |
