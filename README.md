# Carbon Forum HTTP API Documentation
Carbon Forum HTTP API Documentation.

When you are use API, you need to setting api path first.Set up a new website site like `https://api.example.com`, and fill in the path on the page `htttps://your.websit.com/dashboard#dashboard3`. Fill in the path to this line `客户端API域名`

### Guide
* [API Authentication description](authentication.md)
* [User Authentication description](login.md)
* [Public error code](error_code.md)

### API List
Name|Description
---|---
[/page/{{page}}](home.md)|Get topic list
[/login](login.md)|Login (User Authentication description)
[/seccode](seccode.md)|Seccode
[/new](new.md)|Create new topic
[/notifications](notifications.md)|Get notifications list
[/register](register.md)|Register
[/reply](reply.md)|Reply to a topic
[/t/{{topic_id}}-{{page}}](topic.md)|Get the topic information and replies
[/avater](avater.md)|Avater
