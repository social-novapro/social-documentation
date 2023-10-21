# developerAppToken
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | This is a unique string to keep track of who is using your application. |
| userID | string | true | This is used for everything within the site, it's used for posts, live chat, etc. |
| devToken | string | true | This links to your [developerToken](./developerToken.md), it is used to verify you have a proper account. |
| appName | string | false | appName, (old tokens wont have the name) |
| APIUses | number | true | This is the amount of times your application was used. |
| creationTimestamp | string | true | This is the timestamp that your application was created. |