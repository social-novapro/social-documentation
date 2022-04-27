## interactPostSchema
| Field | Type | Optional | Description |
| -- | -- | -- | -- |
| _id | String | false |  Unqiue identifer for the posts.  |
| userID | String | false | This is used for everything within the site, it's used for posts, live chat, etc. |
| timePosted | String | false | Timestamp when the post was created. |
| content | String | false | The content of the post. |
| totalLikes | Number | false | Amount of likes the post has. |
| totalReplies | Number | false | Amount of replies the post has. |
| edited | Boolean | true | Defines if the post was edited. |
| editedTimestamp | String | true | What timestamp was the latest edit. |
| amountEdited | String | true | The amount of times the post was edited. |
| quoteReplyID | String | true | The ID of the post the user quoted. |
| quotedPost | Object<[interactPostSchemaForQuote](#interactpostschemaforquote)> | true | This is a basic data of the quoted post. |
| quotedUser | Object<[interactUserSchemaForQuote](#interactuserschemaforquote)> | true | This is a basic data of the quoted post's user. |

### interactPostSchemaForQuote
| Field | Type | Optional | Description | 
| -- | -- | -- | -- |
| _id | String | false | The quoted postID.|
| userID | String | false | The userID of the user who created the quoted post. |
| timePosted | String | false | Timestamp when the quoted post was created. |
| content | String | false | The content of the quoted post. |
| totalLikes | Number | false | Amount of likes the quoted post has. |
| edited | Boolean | true | Defines if the quoted post was edited. |
| editedTimestamp | String | true | What timestamp was the latest edit of the quoted post.. |
| amountEdited | String | true | The amount of times the quoted post was edited. |


### interactUserSchemaForQuote
| Field | Type | Optional | Description | 
| -- | -- | -- | -- |
| _id | String | false |  userID: this is used for everything within the site, it's used for posts, live chat, etc. |
| username | String | false | Used as a unqiue identifier, someone can search up a username and get the exact result when needed.
| lastEditUsername | String | false | This is used to know the last time they updated their displayname. (also used for rate limiting) |
| displayName | String | false | Used for general name incase username is not as you wanted. |
| description | String | true | The quoted user's bio/description. |
| pronouns | String | true | The quoted user's pronouns. |
| statusTitle | String | true | Users can set a status that shows up on the profile.
| lastEditDisplayname | Number | false | This is used to know the last time they updated their displayname. (also used for rate limiting) |
| creationTimestamp | String | false | When the quoted user first joined the site. |
| followerCount | Number | false | Amount of followers the quoted user has. |
| likeCount | Number | false | Amount of likes the quoted user has on all their posts. |
| likedCount | Number | true | Amount of posts the quoted user has liked |
| totalPosts | Number | true | The total amount of indepentant posts the quoted user has made. |
| totalReplies | Number | true | The total amount of replies the quoted user has made. |
| privacySetting | Object<[privacySettingSchema](#privacysettingschema)> | true | User privacy settings. |

### privacySettingSchema
| Field | Type | Optional | Description | 
| -- | -- | -- | -- |
| discoverySetting | Number<[options](#privacysettingoptions)>| true | Can you search the user up? | 
| postVisiblityDefault | Number<[options](#privacysettingoptions)> | true | Can anybody see the posts? |
| postReplyDefault | Number<[options](#privacysettingoptions)>| true | Can anybody any replies? |


### privacySettingOptions
| Option | Description |
| -- | -- | 
| 1 | Public | Everybody will be able to view data.
| 2 | Friends of Friends Only | Only friends of friends will be able to view data.
| 3 | Private (Friends Only) | Only your friends will be able to view data.
