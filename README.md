# Carbon-Forum-API-Documentation
Carbon Forum HTTP API Documentation.

### Notice
**All API must be called with POST method.**
* [Authentication description](authentication.md)
* [Public error code](error_code.md)

### API List

Name|Description
---|---
[/page/{{page}}](home.md)|Get topic list
[/login](login.md)|Login
[/new](new.md)|Create new topic
[/notifications](notifications.md)|Get notifications list
[/register](register.md)|Register
[/reply](reply.md)|Reply to a topic
[/t/{{topic_id}}-{{page}}](topic.md)|Get the topic information and replies
