# interactPollVoteSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | pollVoteID, linked inside pollVoteIndex |
| _version | number | true | version of pollVote |
| pollID | string | true | pollID |
| userID | string | true | userID |
| lastEdited | number | false | time last changed |
| timestamp | number | true | time voted |
| pollIndexID | string | true | indexID |
| pollOptionID | string | true | pollOptionID |
