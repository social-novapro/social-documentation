# interactAdminSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID |
| adminType | number | true | rank of admin |
| timestamp | number | true | time of acceptance into admin |
| lastReviewID | string | false | link to review schema |

```
/* ranks
    3 | owner
    2 | Super Admin | Can do anything
        can put admin under review
    2 | Admin | Can do anything except delete other admins
        can delete users 
    1 | Moderator 
        can delete posts, comments, and can put users on probation for admin review
    0 | nothing (shouldnt be saved) 
    Can do anything except delete other admins and moderators
*/

/*  lastReview
    _id: id of review
    timestamp: time of review
    userID: id of user in review
    userReviewID: id of review
*/
```
