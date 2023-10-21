## interactPostBookmarks
| Field | Type | Optional | Description |
| -- | -- | -- | -- |
| _id | String | false | This is a unique string, it matches a provided userID. |
| __v | Number | false | This is the version number of the database. |
| lists | Array<[bookmarkLists](#bookmarklists)> | false | The names of every bookmark list user has saved. |
| lists | Array<[bookmarks](#bookmarks)> | false | All the posts saved by the User.  |

### bookmarkLists
| Field | Type | Optional | Description |
| -- | -- | -- | -- |
| _id | String | false | The unique string for the list, independant from the name. | 
| name | String | false | The name of user's list. |
| timestamp | Number | false | Timestamp the list was created. |

### bookmarks
| Field | Type | Optional | Description |
| -- | -- | -- | -- |
| _id | This is the unique string of the post which was saved. | 
| bookmarkList | Name of the list which post is saved in. |
| timestamp | Number | false | Timestamp the post was saved. |
