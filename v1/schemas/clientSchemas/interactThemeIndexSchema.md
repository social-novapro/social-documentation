# interactThemeIndexSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | themeID |
| timestamp | number | true | time created |
| nextID | string | false | next themeID |
| prevID | string | false | prev themeID |
| amount | number | true | amount of themes |
| themeIDs | [themeIndexSchema[]](#themeindexschema) | true | array of themeIDs |

## themeIndexSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | themeID |