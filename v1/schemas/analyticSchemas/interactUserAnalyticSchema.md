# interactUserAnalyticSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true |
| userConnections | [userConnectionsSchema[]](#userconnectionsschema) | false |

## userConnectionsSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | Unique identifier | 
| timestamp | string | true | The timestamp the user made the connection |
| api_urlbase | string | true | The url the user was connected to. This does not include which ID, ex: /v1/get/user/~~:userid~~ |
| api_url | string | true | The url the user was connected to. This includes which ID, ex: /v1/get/user/:userid |

