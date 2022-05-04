# Interact API - v1
Base URL ``https://interact-api.novapro.net/``

## Routes /v1/auth

| # | Name | Description |
| -- | -- | -- |
| 1 | [GET /v1/auth/userLogin](./auth/userlogin/readme.md) | Users can login via this link, and it returns important tokens while using Interact. |
| 2 | [GET /v1/auth/checkToken](./auth/checktoken/readme.md) | You may test the tokens returned with Route #1|

## Routes /v1/delete

| # | Name | Description |
| -- | -- | -- |
| 3 | [DELETE /v1/delete/removePost](./delete/removePost/readme.md) | You are able to remove previously uploaded posts. |

## Routes /v1/get

| # | URL | Description |
| -- | -- | -- |
| 4 | [GET /v1/get/allPosts](./get/allPosts/readme.md) | You can get all posts in Interact. `Will be removed later.` |
| 5 | [GET /v1/get/allPublicData](./get/allPublicData/readme.md) | You can get all users and posts in Interact. `Will be removed later.` |
| 6 | [GET /v1/get/allUsers](./get/allUsers/readme.md)| `not done docs` |
| 7 | [GET /v1/get/analyticTrend](./get/analyticTrend/readme.md) | `not done docs` |
| 8 | [GET /v1/get/post](./get/post/readme.md) | `not done docs` |
| 9 | [GET /v1/get/search](./get/search/readme.md) | `not done docs` |
| 10 | [GET /v1/get/user](./get/user/readme.md) | `not done docs` |
| 11 | [GET /v1/get/userByID](./get/userByID/) | `not done docs` |
| 12 | [GET /v1/get/userFeed](./get/userFeed/readme.md) | `not done docs` |
| 13 | [GET /v1/get/username](./get/username) | `not done docs` |
| 14 | [GET /v1/get/post](./get/post/readme.md) | `not done docs` |

## Routes v1/post

| # | Name | Description |
| -- | -- | -- |
| 15 | [POST /v1/post/createPost](./post/createPost/readme.md) | `not done docs` |

## Routes v1/put

| # | Name | Description |
| -- | -- | -- |
| 16 | PUT /v1/put/editDisplayname | `not done docs` |
| 17 | PUT /v1/put/editPost | `not done docs` |
| 18 | PUT /v1/put/editUsername | `not done docs` |
| 19 | PUT /v1/put/likePost | `not done docs` |

## Routes v1Priv/post

| # | Name | Description |
| -- | -- | -- |
| 20 | POST /v1Priv/post/newAppToken | `not done docs` |
| 21 | POST /v1Priv/post/newDev | `not done docs` |
| 22 | POST /v1Priv/post/newUser | `not done docs` |
