# developerToken
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | This is a unique string to keep track of your developer profile. This is also known as devToken. |
| userID | string | true | This is used for everything within the site, it's used for posts, live chat, etc. |
| premium | boolean | true |
| APIUses | number | true | This is the amount of times your developer token was used. |
| creationTimestamp | string | true | This is the timestamp that your developer account was created. |
| apps | string[] | false | links to appToken | This keeps track of all your applications | 
