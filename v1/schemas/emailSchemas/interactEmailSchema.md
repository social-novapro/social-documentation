# interactEmailSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | unique ID, emailID |
| timestamp | number | true | time created |
| failed | boolean | true | if email failed to send |
| users | userSend[] | true | array of users to send to |
| type | number | true |
| subject | string | true | subject of email |
| content | string | false | content of email |
| html | htmlElement | false | html content of email |


## htmlElement
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | uuid, auto gen |
| h1 | string | false | h1 element |
| p | string | false | p element |
| a | string | false | a element |
| ahref | string | false | a href element |

## userSend
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | false | userID |
| email | string | false | email |
| failed | boolean | true | if email failed to send |
| isBCC | boolean | true | if email is BCC |


```
email.type
    0X = user
        00 = email verification
        01 = welcome
        02 = password reset
            hidden content
    1X = Post
        10 = new post
        11 = post edited
        12 = post deleted
    2X = DM
        20 = new dm
            hidden content
        21 = dm request
            hidden content
    3x = mention
        30 = new mention
        31 = someone replied to your post
        32 = someone liked your post
        33 = someone quoted your post
    4x = notification
        40 = user posted
        41 = notification request
    5x = other
        50 = other  
        51 = unknown
    0= default email
    1= password reset request
    2= dm notification
    3= post notificatoin
    4= mention notification
``````