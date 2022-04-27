# userLogin

``GET /v1/auth/userLogin/``
| required (headers) | type | optional |
| -- | -- | -- |
| devtoken | String | false |
| apptoken | String | false |
| username | String | false |
| password | String | false |

| returned | type | 
| -- | -- |
| accessToken | String |
| userToken | String |
| userID | String |
| publicData | [publicData](../../schemas/interactUserSchema.md) | 
| login | Boolean | 