# interactPollVoteIndexSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | pollVoteIndexID |
| _version | number | true | version of pollVoteIndex |
| timestamp | number | true | time created |
| votes | [voteSchema[]](#voteschema) | true | array of votes |
| previousIndexID | string | false | previous pollVoteIndexID |
| nextIndexID | string | false | next pollVoteIndexID |

### voteSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | pollVoteID |
