# interactDmsMessagesSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | messageID |
| indexID | string | true | indexID |
| userID | string | true | userID |
| groupID | string | true | groupID |
| content | string | true | content of message |
| timestamp | string | true |
| edits | editsObj[] | false | array of editsObj |

## editsObj
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true |
| newContent | string | true |
| oldContent | string | true |
| timestamp | number | true | time edited |
