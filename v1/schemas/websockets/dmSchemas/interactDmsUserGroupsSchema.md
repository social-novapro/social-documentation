# interactDmsUserGroupsSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true |
| groups | groupObj[] | false |
| rooms | groupObj[] | false |
| lastOpened | string | true |

## groupObj
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | group id |
| timestamp | number | true | time entered |
| notifications | number | true | 1: on, 2: off, 3: mentions, 4: default |
| timeLeft | number | false |
