# interactFollowSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID (of person who got followed) |
| follow | [userFollow[]](#userfollow) | false | array of userFollow |

## userFollow
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID (of person who followed) |
| timestamp | number | true | time followed |

```this is unused in the frontned, and will get an overhall in the future```