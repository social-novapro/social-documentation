# interactNotifications
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | notificationID |
| timestamp | number | true | time created |
| type | number | true | type of notification |
| userID | string | true | userID of user who received notification |
| postID | string | false | postID of post related to notification |

```
_id: notificationID
timestamp: Num

type: String (one)
    1: someone followed
    2: someone unfollowed
    3: someone liked post
    4: someone unliked post
    5: someone posted
    6: someone mentioned you
    7: someone quoted your post
type1: Object
    userID
type2: Object
    userID
type3:
    userID
    postID
type4:
    userID
    postID
type5:
    userID
    postID
type6: 
    userID
    postID
```