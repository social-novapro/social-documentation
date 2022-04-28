# checkToken

``GET /v1/auth/checkToken/``
| location | required | type | optional |
| -- | -- | -- | -- |
| header | devtoken | String | false |
| header | apptoken | String | false |
| header | accesstoken | String | false |
| header | usertoken | String | false |
| header | userid | String | false |


| returned | type | 
| -- | -- |
| accessToken | String |
| userToken | String |
| userID | String |
| publicData | [publicData](../../schemas/interactUserSchema.md) | 
| login | Boolean | 