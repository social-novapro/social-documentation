# interactPollSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | pollID |
| _version | number | false |
| timestamp | number | true | time posted |
| userID | string | true | userID of original |
| postID | string | false | main linked PostID (can be linked to other posts) |
| timestampEnding | number | true | time poll ends |
| lastEdited | number | false | time last edited |
| pollName | string | true |
| pollOptions | pollOptions[] | true | array of pollOptions |

### pollOptions
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | false | pollOptionID |
| optionTitle | string | false |
| timestamp | number | false | time added option (maybe can add option later) |
| currentIndexID | string | false | pollVoteIndexID (changes) |
| amountVoted | number | false | amount of votes |
