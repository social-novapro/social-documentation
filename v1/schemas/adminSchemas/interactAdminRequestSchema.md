# interactAdminRequestSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID |
| content | string | true | description of request |
| timestamp | number | true | time requested |
| adminType | number | true | level of request |
| dismissed | number | true | 0 = not dismissed, 1 = dismissed |
| acceptedBy | string | false | id of admin who accepted request |
| acceptedTimestamp | number | false | time request was accepted |