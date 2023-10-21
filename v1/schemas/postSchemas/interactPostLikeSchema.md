# interactPostLikeSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | postID |
| peopleLiked | likeSchema[] | false | array of likeSchema |

## likeSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID of person who liked |
| timeStamp | string | true |
