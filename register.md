# Register

###  HTTP request address
`http://api.example.com/register`


### Menthod
POST


### Notice
You must first request the verification code(`http://api.example.com/seccode.php`), and save the Cookie in the HTTP Header that be returned by the verification code. 

This Cookie should be attached to the HTTP Header when you send the register parameters.


### Parameters
Key|Value Type|Description|Obligatory|Default value
---|---|---|---|---
[API Authentication parameter](authentication.md#parameters)|||√|
UserName|String|Username|√|
Email|String|Email|√|
Password|String(32)|md5(password)|√|
VerifyCode|int(4)||√|null


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
	"ErrorCode": 104001,
	"ErrorMessage": "Forms can not be empty. "
}
```

### Error Code
Error Code|Error Message
---|---
104001|Forms can not be empty. 
104002|Invalid username.
104003|Invalid Email.
104004|Verification code error.
104005|This username already exists. 


###  User Authentication Parameters
Key|Value Type|Description|Obligatory|Example
---|---|---|---|---
AuthUserID|int|UserID|√|173
AuthUserExpirationTime|int(10)|The expiration time of these parameters. |√|1450030066
AuthUserCode|String(32)|Access Token.|√|17cdbe3956a3b87428a080e5361f6f5e

When the API requires user authentication, you need to send the following parameters.
