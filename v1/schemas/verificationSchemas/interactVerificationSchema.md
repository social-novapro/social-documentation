# interactVerificationSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID |
| content | string | true | description of request |
| timestamp | string | true | time requested |
| dismissed | number | true | 0 = not dismissed, 1 = dismissed |
| acceptedBy | string | false | id of admin who accepted request |
| acceptedTimestamp | string | false | time request was accepted |