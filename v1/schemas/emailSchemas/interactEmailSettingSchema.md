# interactEmailSettingSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | userID |
| email | string | true | email address |
| notifications | boolean | true | if email should receive ANY notifications |
| emailSub | boolean | true | if email should receive sub notifications |
| emailNewsLetter | boolean | true | if email should receive newsletter |
| emailAlerts | boolean | true | if email should receive alerts |
| emailReplies | boolean | true | if email should receive replies |
| emailMentions | boolean | false | if email should receive mentions |