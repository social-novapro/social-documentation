## interactAdminErrorIndexSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true |
| amount | number | true |
| timestamp | number | true |
| prevIndexID | string | false |
| nextIndexID | string | false |
| errorIssues | [errorIndexSchema[]](#errorindexschema) | false |

## errorIndexSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true |