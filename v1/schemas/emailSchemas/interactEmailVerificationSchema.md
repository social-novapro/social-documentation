# interactEmailVerificationSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | emailVerID |
| userID | string | true | userID |
| timestamp | number | true | time created email settings |
| timestampVerified | number | false | time verified |
| verified | boolean | true | if email is verified |
| email | string | true | email address |
| replaceCurrent | boolean | true | if email should replace current email |
| replaceEmail | string | false | email to email field with |
| emailHistory | [emailHistoryData[]](#emailhistorydata) | true | email history |
| verificationID | string | false | verification ID sent to email |
| timestampVerSent | number | false | time verification sent |
| shouldRemoveEmail | boolean | false | email should be removed |
| removeEmailVerID | string | false | emailVerID to remove |
| timestampRemoveEmail | number | false | time remove email requested |
| shouldDelAcc | boolean | false | if account should be deleted |
| deleteAccountVerID | string | false | delAccVerID |
| timestampDeleteAccount | number | false | time delete account requested |
| shouldForgotPass | boolean | false | if user knows password |
| shouldChangePass | boolean | false | if user does not know the password |
| replacePassVerID | string | false | passVerID |
| timestampReplacePass | number | false | time replace password requested |

## emailHistoryData
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true |
| timestamp | number | true | time verfied |
| removedTimestamp | number | false | time removed |
| verified | boolean | false | if email is verified |
| email | string | false | email address |
