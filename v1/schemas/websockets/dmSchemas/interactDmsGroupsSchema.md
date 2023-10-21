# interactDmsGroupsSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | groupID |
| groupName | string | true | name of group |
| users | [userObj[]](#userobj) | true | array of userObj |
| owner | string | true | userID |
| created | number | true | date created |
| currentIndex | string | true | indexID |
| notifications | number | true | 1: on, 2: off, 3: mentions |

## userObj
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID |
| timestampJoined | number | true | date joined |
