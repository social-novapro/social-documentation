# interactPostSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | Unqiue identifer for the posts. |
| userID | string | true | userID of poster, this is used for everything within the site, it's used for posts, live chat, etc. |
| timePosted | string | true | Timestamp when the post was created. |
| content | string | false | The content of the post. |
| totalLikes | number | false | Amount of likes the post has. |
| totalReplies | number | false | Amount of replies the post has. |
| totalQuotes | number | false | Amount of quotes the post has. |
| privacySetting | [privacySettingSchema](#privacysettingschema) | false | privacySetting |
| edited | boolean | false | Defines if the post was edited. |
| editedTimestamp | string | false | What timestamp was the latest edit. |
| editedAmount | number | false | The amount of times the post was edited. |
| isQuote | boolean | false | Is the post a quote of another post. |
| quoteData | postQuoteSchema | false | PostID and UserID of quoted post. |
| quoteIndexID | string | false | Current indexID of quotes for this post. |
| isReply | boolean | false | isReply |
| replyData | [postReplySchema](#postreplyschema) | false | replyData |
| replyIndexID | string | false | Current indexID of replies for this post. |
| deleted | boolean | false | Is the post deleted or not |
| hasPoll | boolean | false | hasPoll |
| pollID | string | false | ID of poll that was linked in post. |
| hasMentions | boolean | false | Does the post have mentions. |
| mentionData | [mentionDataSchema[]](#mentiondataschema) | false | Which users were mentioned. |
| quoteReplyPostID | string | false | legacy |
| replyingPostID | string | false | legacy |
| liked | boolean | false | if client liked post (unused) |
| pinned | boolean | false | pinned | if client liked post (unused) |

# postQuoteSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| indexID | string | true | indexID of quoted post. |
| postID | string | true | postID of quoted post. |
| userID | string | true | userID of quoted post. |

# postReplySchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| indexID | string | true | indexID of reply post. |
| postID | string | true | postID of reply post. |
| userID | string | true | userID of reply post. |

# mentionDataSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| userID | string | true | userID of mentioned user. |
| username | string | true | username of mentioned user. |
| index | number | true | index of mention in post. |

# privacySettingSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| discoverySetting | Number<[options](#privacysettingoptions)>| false | Can you search the user up? |
| postVisiblityDefault | Number<[options](#privacysettingoptions)> | false | Can anybody see the posts? |
| postReplyDefault | Number<[options](#privacysettingoptions)>| false | Can anybody any replies? |


### privacySettingOptions
| Option | Description |
| -- | -- | 
| 1 | Public | Everybody will be able to view data.
| 2 | Friends of Friends Only | Only friends of friends will be able to view data.
| 3 | Private (Friends Only) | Only your friends will be able to view data.
