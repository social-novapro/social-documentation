# Interact API - v1
Base URL ``https://interact-api.novapro.net/``

## 1: Routes /v1/auth

| # | Name | Description |
| -- | -- | -- |
| 1.1 | [GET /v1/auth/userLogin](./auth/userlogin/readme.md) | Users can login via this link, and it returns important tokens while using Interact. |
| 1.2 | [GET /v1/auth/checkToken](./auth/checktoken/readme.md) | You may test the tokens returned with Route #1|

## 2: Routes /v1/delete

| # | Name | Description |
| -- | -- | -- |
| 2.1 | [DELETE /v1/delete/removePost](./delete/removePost/readme.md) | You are able to remove previously uploaded posts. |
| 2.2 | [DELETE /v1/delete/unfollowUser](./delete/unfollowUser/readme.md) | Let client unfollow a previously followed user. |
| 2.3 | [DELETE /v1/delete/unlikePost](./delete/unlikePost/readme.md) | Let client unlike a previously liked post. |
| 2.3 | [DELETE /v1/delete/unsubUser](./delete/unsubUser/readme.md) | Let client unsub to user notifications. |

## 3: Routes /v1/get

| # | URL | Description |
| -- | -- | -- |
| 3.1 | [GET /v1/get/allPosts](./get/allPosts/readme.md) | You can get all posts in Interact. `Will be removed later.` |
| 3.2 | [GET /v1/get/allPublicData](./get/allPublicData/readme.md) | You can get all users and posts in Interact. `Will be removed later.` |
| 3.3 | [GET /v1/get/allUsers](./get/allUsers/readme.md)| You can get all users in Interact. `Will be removed later.` |
| 3.4 | [GET /v1/get/analyticTrend](./get/analyticTrend/readme.md) | You can get all API requests done by all users. `Will be removed later.` |
| 3.5 | [GET /v1/get/post](./get/post/readme.md) | You can get info on a specific post. |
| 3.6 | [GET /v1/get/search](./get/search/readme.md) | You can search for a post on Interact. |
| 3.7 | [GET /v1/get/user](./get/user/readme.md) | You can get info on a specific user by their username. |
| 3.8 | [GET /v1/get/userByID](./get/userByID/) | You can get info on a specific user by their user ID. |
| 3.9 | [GET /v1/get/userFeed](./get/userFeed/readme.md) | You can get all posts created by a specific user. |
| 3.10 | [GET /v1/get/username](./get/username) | You can get info on a specific user by their username. | <!-- this api is redundant, as /v1/get/user supplies the same information as well as some more -->
| 3.11 | [GET /v1/get/bookmarks](./get/bookmarks) | Fetch bookmakrs saved by client. | 
| 3.12 | [GET /v1/get/developer](./get/developer) | Fetch developer data of a client. | 
| 3.13 | [GET /v1/get/followers](./get/followers) | Fetch followers of a user.  | 
| 3.14 | [GET /v1/get/following](./get/following) | Fetch who a user is following. | 
| 3.15 | [GET /v1/get/notifications](./get/notifications) | Fetch notifications of a client. | 
| 3.16 | [GET /v1/get/postEditHistory](./get/postEditHistory) | Fetch edit history of a post. | 
| 3.17 | [GET /v1/get/postLikedBy](./get/postLikedBy) | Fetch who liked a post. | 
| 3.19 | [GET /v1/get/subscriptions ](./get/subscriptions) |  Fetch who a client is subscribed to. | 


## 4: Routes v1/post

| # | Name | Description |
| -- | -- | -- |
| 4.1 | [POST /v1/post/createPost](./post/createPost/readme.md) | You can create a post on Interact. |
| 4.2 | [POST /v1/post/requestVerify](./post/requestVerify/readme.md) | You can request verification for a user account. |

## 5: Routes v1/put

| # | Name | Description |
| -- | -- | -- |
| 5.1 | PUT /v1/put/userEdit | You can edit user data. |
| 5.2 | PUT /v1/put/editPost | You can edit a post. |
| 5.3 | PUT /v1/put/likePost | You can like a post. |
| 5.4 | PUT /v1/put/editDisplayname | You can edit a user's display name. |
| 5.5 | PUT /v1/put/editUsername | You can edit a user's username. |

## 6: Routes v1Priv/post

| # | Name | Description |
| -- | -- | -- |
| 6.1 | POST /v1Priv/post/newAppToken | You can create an application token. You need dev, app, and user tokens to perform API calls.|
| 6.2 | POST /v1Priv/post/newDev | You can create a development token. You need dev, app, and user tokens to perform API calls.|
| 6.3 | POST /v1Priv/post/newUser | You can create a new user |
