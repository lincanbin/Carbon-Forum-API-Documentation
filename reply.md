# Reply to topic

###  HTTP request address
`http://api.example.com/reply`

### Menthod
POST

###  Parameters
Key|Value Type|Description|Obligatory|Default value
---|---|---|---|---
[API Authentication parameter](authentication.md#parameters)|||√|
[User Authentication parameter](login.md#user-authentication-parameters)|||√|
TopicID|int||√|0
Content|String||√|null


### HTTP Response
Success:
```json
{
	"Status": 1,
	"TopicID": 12,
	"PostID": 450,
	"Page": 1 /* Total page of this topic. */
}
```

Fail:
```json
{
	"Status": 0,
	"ErrorCode": 102001,
	"ErrorMessage": "Content empty. "
}
```

### Error Code
Error Code|Error Message
---|---
102001|Content empty. 
102002|Content is too long
