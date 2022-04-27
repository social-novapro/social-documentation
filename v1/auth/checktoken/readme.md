# checkToken

``GET /v1/auth/checkToken/``
| required (headers) | type | optional |
| -- | -- | -- |
| devtoken | String | false |
| apptoken | String | false |
| accesstoken | String | false |
| usertoken | String | false |
| userid | String | false |


| returned | type | 
| -- | -- |
| accessToken | String |
| userToken | String |
| userID | String |
| publicData | [publicData](../../schemas/interactUserSchema.md) | 
| login | Boolean | 