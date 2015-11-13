# Create new topic

###  HTTP request address
`http://api.example.com/new`

### Menthod
POST

###  Parameters
Key|Value Type|Description|Obligatory|Default value
---|---|---|---|---
[API Authentication parameter](authentication.md#parameters)|||√|
[User Authentication parameter](login.md#user-authentication-parameters)|||√|
Title|String||√|
Tag[]|String|If you need to add a number of tags, you can call this parameter repeatedly.|√|
Content|String||×|null


### HTTP Response
Success:
```json
{
	"Status": 1,
	"TopicID": 12450
}
```

Fail:
```json
{
	"Status": 0,
	"ErrorCode": 103001,
	"ErrorMessage": "Title can't be empty. "
}
```

### Error Code
Error Code|Error Message
---|---
103001|Title can't be empty
103002|Content is too long
103003|Tag can't be empty
