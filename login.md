# Login

###  HTTP request address
`http://api.example.com/login`


### Menthod
POST


### Notice
You must first request the verification code(`http://api.example.com/seccode.php`), and save the Cookie in the HTTP Header that be returned by the verification code. 

This Cookie should be attached to the HTTP Header when you send the login parameters.


### Parameters
Key|Value Type|Description|Obligatory|Default value
---|---|---|---|---
[API Authentication parameter](authentication.md)|||√|
UserName|String|Username|√|
Password|String|password|√|
VerifyCode|int(4)||√|null
VerifyCode|int(2)|The validity period of the token acquired. Default value is 30 days. |×|30


### HTTP Response
Success:
```json
{
    "Status": 1,
    "UserID": 173,
    "UserExpirationTime": 1450030066,
    "UserCode": "17cdbe3956a3b87428a080e5361f6f5e",
    "UserInfo": {
        "ID": 173,
        "UserName": "lincanbin",
        "UserRoleID": 5,
        "UserMail": "lincanbin@hotmail.com",
        "UserIntro": "一个穷人。"
    }
}
```

Fail:
```json
{
	"Status": 0,
	"ErrorCode": 101001,
	"ErrorMessage": "Forms can not be empty. "
}
```

### Error Code
Error Code|Error Message
---|---
101001|Forms can not be empty. 
101002|Verification code error. 
101003|User does not exist. 
101004|Password error.


###  User Authentication Parameters
Key|Value Type|Description|Obligatory|Example
---|---|---|---|---
AuthUserID|int|UserID|√|173
AuthUserExpirationTime|int(10)|The expiration time of these parameters. |√|1450030066
AuthUserCode|String(32)|Access Token.|√|17cdbe3956a3b87428a080e5361f6f5e

When the API requires user authentication, you need to send the following parameters.
