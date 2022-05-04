# allPosts

``GET /v1/get/analyticTrend/``

[Example of Request](#example-of-request)

## Required 
| location | required | type | optional |
| -- | -- | -- | -- |
| header | devtoken | String | false |
| header | apptoken | String | false |
| header | accesstoken | String | false |
| header | usertoken | String | false |
| header | userid | String | false |

## Returned Data
| returned | type | 
| -- | -- |
| Array | Array<[eachUser](#each-user)> |


### Each User
| Field | Type | Optional | Description |
| -- | -- | -- | -- |
| _id | String | false | This is the UserID for the Object of connections. |
| __v | Number | false | Version Number of saved result. |
| userConnections | Array<[eachReq](#each-request)> | false | 


### Each Request
| Field | Type | Optional | Description |
| -- | -- | -- | -- |
| _id | String | false | Random UID, users could delete eventually. |
| timestamp | String | false | Timestamp made at time of connection. |
| api_urlbase | String | false | URL of request. |
| api_url | String | false | URL of request, including param. |

## Example of Request
### Request
Request URL

``GET https://interact-api.novapro.net/v1/get/analyticTrend``

JavaScript Request Example
```js
const headers = {
    devtoken: "XXXX",
    apptoken: "XXXX",
    userid: "XXXX",
    usertoken: "XXXX",
    accesstoken: "XXXX"
}

const response = await fetch(`https://interact-api.novapro.net/v1/get/analyticTrend`, { method: 'GET', headers})

var data = await response.json() 
```

### Returned Data
``` JSON
[
	{
		"_id": "6ceae342-2ca2-48ec-8ce3-0e39caebe989",
		"__v": 0,
		"userConnections": [
			{
				"_id": "81b0f0a4-9efe-47cb-98da-c3bb64cfff13",
				"timestamp": "1647282601254",
				"api_urlbase": "/v1/post/createPost",
				"api_url": "/v1/post/createPost"
			},
			{
				"_id": "bcb67940-6e35-4dde-abd2-bb4deaea0864",
				"timestamp": "1647282604678",
				"api_urlbase": "/v1/get/search",
				"api_url": "/v1/get/search/"
			},
			{
				"_id": "5bdc4b25-245f-467e-b563-d4e48b83f4d0",
				"timestamp": "1647282643502",
				"api_urlbase": "/v1/get/post",
				"api_url": "/v1/get/post/790919b8-c095-4c81-a515-ec8f8eb72145"
			},
			{
				"_id": "7b43c25c-34b2-4dbe-9bee-7ae43db10c2a",
				"timestamp": "1647282693485",
				"api_urlbase": "/v1Priv/get/userAnalytics",
				"api_url": "/v1Priv/get/userAnalytics/6ceae342-2ca2-48ec-8ce3-0e39caebe989"
			},
		]
	},
	{
		"_id": "2b5bf09d-99ab-4e2b-8191-9b56e88a0608",
		"__v": 0,
		"userConnections": [
			{
				"_id": "c06f4ee0-6e70-4471-82f8-c3babfa7588c",
				"timestamp": "1651377882059",
				"api_urlbase": "/v1/get/allPosts",
				"api_url": "/v1/get/allPosts"
			},
			{
				"_id": "4887e31e-572d-46e0-af79-7fe8c435b3d2",
				"timestamp": "1651377995473",
				"api_urlbase": "/v1/auth/checkToken",
				"api_url": "/v1/auth/checkToken/"
			},
			{
				"_id": "d8280029-e823-4b7a-9831-8de450fb3c0d",
				"timestamp": "1648666724791",
				"api_urlbase": "/v1/auth/checkToken",
				"api_url": "/v1/auth/checkToken/"
			},
		]
	}
]
```