# interactDeletedSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | unique ID, deletedID |
| type | number | true | 1=user, 2=post, .find({_id: userID, type: 1 }) |
| userID | string | true | userID of deleted account or creator |
| username | string | false | username of account |