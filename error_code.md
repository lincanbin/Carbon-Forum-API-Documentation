# Public Error Code
The HTTP response message is accompanied by the same Status Code in HTTP Header when these errors occur. 

### HTTP Response Header
```
HTTP/1.1 403 Forbidden
Status: 403 Forbidden
```
### HTTP Response Body
```json
{
	"Status": 0,
	"ErrorCode": 403,
	"ErrorMessage": "403 Forbidden"
}
```

### Error Code
Error Code|Error Message
---|---
400|Bad Request. Check that your request parameters is consistent with the API documentation.
401|Unauthorized. This API requires [user authentication parameters](login.md#user-authentication-parameters). Parameters error or no given. 
403|Forbidden. [API Authentication parameter](authentication.md#parameters) error or no given.
404|The requested resource does not exist.
500|Internal Server Error
503|Service Unavailable
