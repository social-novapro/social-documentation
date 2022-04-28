# userLogin

``GET /v1/auth/userLogin/``
| location | required | type | optional |
| -- | -- | -- | -- |
| header | devtoken | String | false |
| header | apptoken | String | false |
| header | username | String | false |
| header | password | String | false |

| returned | type | 
| -- | -- |
| accessToken | String |
| userToken | String |
| userID | String |
| publicData | [publicData](../../schemas/interactUserSchema.md) | 
| login | Boolean | 