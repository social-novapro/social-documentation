## interactUserAccessSchema
| Field | Type | Optional | Description |
| -- | -- | -- | -- |
| _id | String | false | This is used to connect a user to an appToken. The user can revoke this accessToken when wanted. This is also known as an accessToken|
| userToken | String | false | This is a token applications can use to verify you. |
| userID | String | false | This is used for everything within the site, it's used for posts, live chat, etc. |
| appToken | Number | false | This is used to match the other request header called appToken. |