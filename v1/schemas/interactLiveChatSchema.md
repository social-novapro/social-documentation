# interactLiveChatSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID |
| type | number | true  |
| user | [userSchema](#userschema) | true |
| apiVersions | string | true |
| pings | [pingsSchema](#pingsschema) | false |
| message | [messageSchema](#messageschema) | false |
| userJoin | [userJoinSchema](#userjoinschema) | false |
| userLeave | [userLeaveSchema](#userleaveschema) | false |

### userSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID |
| username | string | true |
| displayName | string | true |

### pingsSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| alive | boolean | true |

### messageSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| userID | string | true |
| user | string | true |
| currentUsers | string | true |
| content | string | true |
| timeStamp | string | true |
| replyTo | string | true | messageID |
| edited | boolean | true |
| editedTimeStamp | string | true |


### userJoinSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| userID | string | true |
| user | string | true |
| currentUsers | string | true |
| content | string | true |
| timeStamp | string | true |

### userLeaveSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| userID | string | true |
| user | string | true |
| currentUsers | string | true |
| content | string | true |
| timeStamp | string | true |

```there should be a rewrite of live chat eventually, so this schema will be unnecessary```
