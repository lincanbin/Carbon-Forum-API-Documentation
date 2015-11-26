# Get the Topic Information and Replies

###  HTTP request address
`http://api.example.com/t/{{topic_id}}-{{page}}`

### Menthod
GET

### Parameters
Key|Value Type|Description|Obligatory|Default value
---|---|---|---|---
[API Authentication parameter](authentication.md#parameters)|||√|
[User Authentication parameter](login.md#user-authentication-parameters)|||×|
{{topic_id}}|int|Topic ID. This parameter should be constructed in the requests address. |√|
{{page}}|int|Page number of the replies list. This parameter should be constructed in the requests address. |√|


### HTTP Response
Success:
```json

```

Fail:
```json
	"Status": 0,
	"ErrorCode": 404,
	"ErrorMessage": "404 Not Found"
```
