# interactPostEditSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | postID |
| userID | string | true | userID (of person who posts) |
| edits | editSchema[] | false | array of editSchema |

## editSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| publicTimestamp | string | true | time of publish (of last content) |
| removedTimestamp | string | true | time of removal (of content) |
| content | string | true | old content of post |
