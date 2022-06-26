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
| 6 | [GET /v1/get/allUsers](./get/allUsers/readme.md)| You can get all users in Interact. `Will be removed later.` |
| 7 | [GET /v1/get/analyticTrend](./get/analyticTrend/readme.md) | You can get all API requests done by all users. `Will be removed later.` |
| 8 | [GET /v1/get/post](./get/post/readme.md) | You can get info on a specific post. |
| 9 | [GET /v1/get/search](./get/search/readme.md) | You can search for a post on Interact. |
| 10 | [GET /v1/get/user](./get/user/readme.md) | You can get info on a specific user by their username. |
| 11 | [GET /v1/get/userByID](./get/userByID/) | You can get info on a specific user by their user ID. |
| 12 | [GET /v1/get/userFeed](./get/userFeed/readme.md) | You can get all posts created by a specific user. |
| 13 | [GET /v1/get/username](./get/username) | You can get info on a specific user by their username. | <!-- this api is redundant, as /v1/get/user supplies the same information as well as some more -->
| 14 | [GET /v1/get/post](./get/post/readme.md) | You can get info on a specific post. |

## Routes v1/post

| # | Name | Description |
| -- | -- | -- |
| 15 | [POST /v1/post/createPost](./post/createPost/readme.md) | You can create a post on Interact. |
| 16 | [POST /v1/post/requestVerify](./post/requestVerify/readme.md) | You can request verification for a user account. |

## Routes v1/put

| # | Name | Description |
| -- | -- | -- |
| 17 | PUT /v1/put/userEdit | You can edit user data. |
| 18 | PUT /v1/put/editPost | You can edit a post. |
| 20 | PUT /v1/put/likePost | You can like a post. |
| 21 | PUT /v1/put/editDisplayname | You can edit a user's display name. |
| 22 | PUT /v1/put/editUsername | You can edit a user's username. |

## Routes v1Priv/post

| # | Name | Description |
| -- | -- | -- |
| 23 | POST /v1Priv/post/newAppToken | You can create an application token. You need dev, app, and user tokens to perform API calls.|
| 24 | POST /v1Priv/post/newDev | You can create a development token. You need dev, app, and user tokens to perform API calls.|
| 25 | POST /v1Priv/post/newUser | You can create a new user |
