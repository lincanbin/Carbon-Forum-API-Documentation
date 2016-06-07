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
{
    "Status": 1,
    "Page": 1,
    "TotalPage": 2,
    "IsFavorite": 0,
    "TopicInfo": {
        "ID": 4015,
        "Topic": "我的DigitalOcean的VPS终于要退役了，用了一年。",
        "Tags": "DigitalOcean|VPS",
        "UserID": 173,
        "UserName": "lincanbin",
        "LastName": "jetereting",
        "PostTime": 1464833166,
        "LastTime": 1465216707,
        "IsGood": 0,
        "IsTop": 0,
        "IsLocked": 0,
        "IsDel": 0,
        "IsVote": 0,
        "Views": 225,
        "Replies": 24,
        "RatingSum": 0,
        "TotalRatings": 0,
        "LastViewedTime": 1465244974,
        "PostsTableName": null,
        "ThreadStyle": "",
        "Lists": "",
        "ListsTime": 1464833166,
        "Log": "",
        "Favorites": 0
    },
    "PostsArray": [
        {
            "ID": 16952,
            "TopicID": 4015,
            "UserID": 173,
            "UserName": "lincanbin",
            "Content": "<p><img src=\"/upload/image/20160602/1464833075797574.png\" title=\"1464833075797574.png\" alt=\"blob.png\"/></p><p><img src=\"/upload/image/20160602/1464833114973747.png\" title=\"1464833114973747.png\" alt=\"blob.png\"/></p><p>打完这个Snapshot就Destroy，毕竟没钱了。</p>",
            "PostTime": 1464833166,
            "IsDel": 0,
            "PostFloor": 0
        },
        {
            "ID": 16953,
            "TopicID": 4015,
            "UserID": 3646,
            "UserName": "hulu",
            "Content": "<p>我觉得IBM的bluemix不错，免费配额也够用了。\n可以试试</p>",
            "PostTime": 1464835043,
            "IsDel": 0,
            "PostFloor": 1
        },
        {
            "ID": 16954,
            "TopicID": 4015,
            "UserID": 173,
            "UserName": "lincanbin",
            "Content": "<p>回复<a href=\"/goto/4015-16953#Post16953\">#1</a> @hulu :<br/></p><p>我比较挑线路，还需要比较高的自由度。</p>",
            "PostTime": 1464835077,
            "IsDel": 0,
            "PostFloor": 2
        },
        {
            "ID": 16956,
            "TopicID": 4015,
            "UserID": 2530,
            "UserName": "ivanilla",
            "Content": "<p>核电<br/></p>",
            "PostTime": 1464835709,
            "IsDel": 0,
            "PostFloor": 3
        },
        {
            "ID": 16962,
            "TopicID": 4015,
            "UserID": 173,
            "UserName": "lincanbin",
            "Content": "<p>好像不止一年，是一年半了。</p>",
            "PostTime": 1464845195,
            "IsDel": 0,
            "PostFloor": 4
        },
        {
            "ID": 16969,
            "TopicID": 4015,
            "UserID": 2498,
            "UserName": "chenxi",
            "Content": "<p>新的VPS什么配置？内存多大？</p>",
            "PostTime": 1464863372,
            "IsDel": 0,
            "PostFloor": 5
        },
        {
            "ID": 16970,
            "TopicID": 4015,
            "UserID": 173,
            "UserName": "lincanbin",
            "Content": "<p>\n回复 <a href=\"/t/4015#Post16969\">#0</a> @chenxi :<br/>\n</p><p><p>一个月900日元，1G内存，2核CPU。</p>\n</p>",
            "PostTime": 1464863407,
            "IsDel": 0,
            "PostFloor": 6
        },
        {
            "ID": 16971,
            "TopicID": 4015,
            "UserID": 2498,
            "UserName": "chenxi",
            "Content": "<p>回复<a href=\"/goto/4015-16970#Post16970\">#6</a> @lincanbin :<br/></p><p>那鲁好道！ </p>",
            "PostTime": 1464863583,
            "IsDel": 0,
            "PostFloor": 7
        },
        {
            "ID": 16972,
            "TopicID": 4015,
            "UserID": 173,
            "UserName": "lincanbin",
            "Content": "<p>\n回复 <a href=\"/t/4015#Post16971\">#0</a> @chenxi :<br/>\n</p><p><p>真贵啊。</p>\n</p>",
            "PostTime": 1464863704,
            "IsDel": 0,
            "PostFloor": 8
        },
        {
            "ID": 16973,
            "TopicID": 4015,
            "UserID": 2498,
            "UserName": "chenxi",
            "Content": "<p>回复<a href=\"/goto/4015-16972#Post16972\">#8</a> @lincanbin :<br/></p><p>对日本人来说，900日元就是一顿午饭钱 </p>",
            "PostTime": 1464863814,
            "IsDel": 0,
            "PostFloor": 9
        },
        {
            "ID": 16974,
            "TopicID": 4015,
            "UserID": 173,
            "UserName": "lincanbin",
            "Content": "<p>\n回复 <a href=\"/t/4015#Post16973\">#0</a> @chenxi :<br/>\n</p><p><p>对我来说是很多顿</p>\n</p>",
            "PostTime": 1464863890,
            "IsDel": 0,
            "PostFloor": 10
        },
        {
            "ID": 16975,
            "TopicID": 4015,
            "UserID": 2498,
            "UserName": "chenxi",
            "Content": "<p>回复<a href=\"/t/4015#Post16974\">#10</a> @lincanbin :<br/></p><p>你和你女朋友吃顿肯德基也差不多没了。</p><p>楼主回复的帖子全部显示 【回复 #0】 吗？</p>",
            "PostTime": 1464864228,
            "IsDel": 0,
            "PostFloor": 11
        },
        {
            "ID": 16976,
            "TopicID": 4015,
            "UserID": 173,
            "UserName": "lincanbin",
            "Content": "<p>\n回复 <a href=\"/t/4015#Post16975\">#11</a> @chenxi :<br/>\n</p><p><p>因为是用客户端</p>\n</p>",
            "PostTime": 1464864270,
            "IsDel": 0,
            "PostFloor": 12
        },
        {
            "ID": 16977,
            "TopicID": 4015,
            "UserID": 2498,
            "UserName": "chenxi",
            "Content": "<p>硬盘多大的?</p>",
            "PostTime": 1464864280,
            "IsDel": 0,
            "PostFloor": 13
        },
        {
            "ID": 16978,
            "TopicID": 4015,
            "UserID": 173,
            "UserName": "lincanbin",
            "Content": "<p>\n回复 <a href=\"/t/4015#Post16975\">#11</a> @chenxi :<br/>\n</p><p><p>客户端直接在提醒页回复就这样。</p>\n</p>",
            "PostTime": 1464864288,
            "IsDel": 0,
            "PostFloor": 14
        },
        {
            "ID": 16979,
            "TopicID": 4015,
            "UserID": 173,
            "UserName": "lincanbin",
            "Content": "<p>\n回复 <a href=\"/t/4015#Post16977\">#13</a> @chenxi :<br/>\n</p><p><p>50G</p>\n</p>",
            "PostTime": 1464864298,
            "IsDel": 0,
            "PostFloor": 15
        },
        {
            "ID": 16980,
            "TopicID": 4015,
            "UserID": 173,
            "UserName": "lincanbin",
            "Content": "<p>\n回复 <a href=\"/t/4015#Post16975\">#11</a> @chenxi :<br/>\n</p><p><p>我从来都是自己一个人出去吃饭的，跟女朋友一起吃这种事，大概只能在梦里有了。</p>\n</p>",
            "PostTime": 1464864359,
            "IsDel": 0,
            "PostFloor": 16
        },
        {
            "ID": 16981,
            "TopicID": 4015,
            "UserID": 2498,
            "UserName": "chenxi",
            "Content": "<p>回复<a href=\"/t/4015#Post16980\">#16</a> @lincanbin :<br/></p><p>好吧，我是说你的右手。。。 </p>",
            "PostTime": 1464864467,
            "IsDel": 0,
            "PostFloor": 17
        },
        {
            "ID": 16982,
            "TopicID": 4015,
            "UserID": 173,
            "UserName": "lincanbin",
            "Content": "<p>\n回复 <a href=\"/t/4015#Post16981\">#17</a> @chenxi :<br/>\n</p><p><p>你怎么知道我用右手…</p>\n</p>",
            "PostTime": 1464864641,
            "IsDel": 0,
            "PostFloor": 18
        },
        {
            "ID": 16983,
            "TopicID": 4015,
            "UserID": 2498,
            "UserName": "chenxi",
            "Content": "<p>回复<a href=\"/t/4015#Post16982\">#18</a> @lincanbin :</p>\n\n<p>看你打的字，键盘右手侧敲出来的字母明显比左边的字母颜色深很多，所以断定你右手已经不经意间练的很粗壮了。。。hoho</p>",
            "PostTime": 1464866458,
            "IsDel": 0,
            "PostFloor": 19
        }
    ]
}
```

Fail:
```json
	"Status": 0,
	"ErrorCode": 404,
	"ErrorMessage": "404 Not Found"
```
