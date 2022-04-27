## interactUserAnalyticSchema
| Field | Type | Optional | Description |
| -- | -- | -- | -- |
| _id | String | false |  userID: this is used for everything within the site, it's used for posts, live chat, etc. |
| userConnections | Array<[userConnectionsSchema](#userconnectionsschema)> | true | The total amount of indepentant posts the user has made. |

### userConnectionsSchema
| Field | Type | Optional | Description | 
| -- | -- | -- | -- |
| _id | String | true | Unique identifier | 
| timestamp | String | true | The timestamp the user made the connection |
| api_urlbase | String | true | The url the user was connected to. This does not include which ID, ex: /v1/get/user/~~:userid~~ |
| api_url | String | true | The url the user was connected to. This includes which ID, ex: /v1/get/user/:userid |
