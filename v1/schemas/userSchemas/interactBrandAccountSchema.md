# interactBrandAccountSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID (of brand) |
| users | [userBrandSchema[]](#userbrandschema) | false | array of userBrandSchema |

## userBrandSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID (of person who has access) |
| timestamp | number | true | time added |
| accessLevel | number | true | 1: owner, 2: admin, 3: manager, 4: poster |


```
1: owner
    access to everything
2: admin
    access to everything (minus deleting account)
3: manager
    can delete other posts
4: poster
    can post in place of brand account
```