# Get the User Avater

###  HTTP request address
`http://api.example.com/upload/avatar/{{size}}/{{userID}}.png`

### Menthod
GET

### Parameters
Key|Value Type|Description|Obligatory|Default value
---|---|---|---|---
size | string| `large` or `middle` | √ |
userID | string | user id | √


### HTTP Response
Success:
```
User avater response image data. Middle Image size is 48*48.
Large Image size is 256*256.
```

Fail:
* This API does not throw an error now.
