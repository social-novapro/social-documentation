# interactAdminErrorSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true |
| userID | string | true |
| errorVersion | number | true |
| errorCode | string | true |
| errorMsg | string | true |
| timestamp | number | true |
| resolved | boolean | true |
| resolvedTimestamp | number | false |
| inReview | boolean | true |
| reviewedBy | string | false |
| reviewTimestamp | number | false |
| reviewHistory | [reviewHistorySchema[]](#reviewhistoryschema) | false |


## reviewHistorySchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true |
| reviewBy | string | true |
| reviewStart | number | true |
| reviewEnd | number | true |
| resolvedTimestamp | number | false | 
