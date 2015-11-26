# Get Topic List

###  HTTP request address
`http://api.example.com/page/{{page}}`

### Menthod
GET

### Parameters
Key|Value Type|Description|Obligatory|Default value
---|---|---|---|---
[API Authentication parameter](authentication.md#parameters)|||√|
{{page}}|int|Page number of the topic list. This parameter should be constructed in the requests address. |√|


### HTTP Response
Success:
```json
{
    "Status": 1,
    "PageTitle": "Carbon Forum",
    "Page": 1,
    "TotalPage": 85,
    "TopicsArray": [
        {
            "ID": 2465,
            "Topic": "Carbon Forum项目捐赠列表",
            "Tags": "捐赠",
            "UserID": 173,
            "UserName": "lincanbin",
            "LastName": "lincanbin",
            "LastTime": 1453885194,
            "Replies": 92
        },
        {
            "ID": 2652,
            "Topic": "对程序有建议的，可以直接发主题，加“建议”标签",
            "Tags": "功能|建议|标签|程序",
            "UserID": 173,
            "UserName": "lincanbin",
            "LastName": "lincanbin",
            "LastTime": 1451314363,
            "Replies": 30
        },
        {
            "ID": 2389,
            "Topic": "测试发帖回帖功能时，不要拍着键盘就发出来",
            "Tags": "Test|测试|话题",
            "UserID": 173,
            "UserName": "lincanbin",
            "LastName": "zhangzhg0508",
            "LastTime": 1448540419,
            "Replies": 173
        },
        {
            "ID": 3340,
            "Topic": "hh",
            "Tags": "hh",
            "UserID": 173,
            "UserName": "lincanbin",
            "LastName": "lincanbin",
            "LastTime": 1447439151,
            "Replies": 2
        },
        {
            "ID": 3338,
            "Topic": "弄",
            "Tags": "莫",
            "UserID": 173,
            "UserName": "lincanbin",
            "LastName": "lincanbin",
            "LastTime": 1447251326,
            "Replies": 4
        },
        {
            "ID": 3032,
            "Topic": "Carbon Forum 3.6.5 发布，手机版重构大提速 &amp; 新增QQ/微博登陆、话题广场、邮件取回密码等新功能……",
            "Tags": "Carbon Forum|更新",
            "UserID": 173,
            "UserName": "lincanbin",
            "LastName": "布拉皮特",
            "LastTime": 1447211465,
            "Replies": 85
        },
        {
            "ID": 3225,
            "Topic": "又想起了有这么个坑没填了——Android客户端进度",
            "Tags": "Android|客户端|手机",
            "UserID": 173,
            "UserName": "lincanbin",
            "LastName": "admin222",
            "LastTime": 1447210367,
            "Replies": 25
        },
        {
            "ID": 3339,
            "Topic": "454",
            "Tags": "测试",
            "UserID": 1750,
            "UserName": "lincanbin2",
            "LastName": "admin222",
            "LastTime": 1447210360,
            "Replies": 3
        },
        {
            "ID": 3337,
            "Topic": "哦你",
            "Tags": "哦你|咯",
            "UserID": 173,
            "UserName": "lincanbin",
            "LastName": "",
            "LastTime": 1447157281,
            "Replies": 0
        },
        {
            "ID": 3336,
            "Topic": "不",
            "Tags": "谷歌",
            "UserID": 173,
            "UserName": "lincanbin",
            "LastName": "",
            "LastTime": 1447092840,
            "Replies": 0
        },
        {
            "ID": 3335,
            "Topic": "gggg",
            "Tags": "Test|功能|建议|话题",
            "UserID": 173,
            "UserName": "lincanbin",
            "LastName": "lincanbin",
            "LastTime": 1447092779,
            "Replies": 1
        },
        {
            "ID": 3331,
            "Topic": "Cb123导航网专注免费收录Carbon Forum程序网站",
            "Tags": "导航|Cb123导航网",
            "UserID": 485,
            "UserName": "hlbj105",
            "LastName": "hlbj105",
            "LastTime": 1446950587,
            "Replies": 3
        },
        {
            "ID": 3334,
            "Topic": "可以跟ecshop整合马？",
            "Tags": "论坛",
            "UserID": 801,
            "UserName": "qqnet",
            "LastName": "lincanbin",
            "LastTime": 1446912879,
            "Replies": 1
        },
        {
            "ID": 3333,
            "Topic": "jing",
            "Tags": "图片|测试|垃圾信息",
            "UserID": 1746,
            "UserName": "hahaha123",
            "LastName": "",
            "LastTime": 1446906234,
            "Replies": 0
        },
        {
            "ID": 3332,
            "Topic": "cf可否稳定常用？楼主基本小白，只玩过dz，但是越来越臃肿了···只需要交流，别的都是多余的",
            "Tags": "问题",
            "UserID": 1744,
            "UserName": "布鲁斯叔叔",
            "LastName": "布鲁斯叔叔",
            "LastTime": 1446899767,
            "Replies": 3
        },
        {
            "ID": 2885,
            "Topic": "林先生今天找到女朋友了吗？",
            "Tags": "女朋友|打卡",
            "UserID": 173,
            "UserName": "lincanbin",
            "LastName": "lincanbin",
            "LastTime": 1446886895,
            "Replies": 161
        },
        {
            "ID": 3329,
            "Topic": "我的话题数量一直 是1什么情况",
            "Tags": "问题|话题",
            "UserID": 1731,
            "UserName": "情趣",
            "LastName": "lincanbin",
            "LastTime": 1446875010,
            "Replies": 1
        },
        {
            "ID": 3330,
            "Topic": "关于附件下载权限的问题",
            "Tags": "附件|权限|建议",
            "UserID": 1511,
            "UserName": "尤里卡",
            "LastName": "lincanbin",
            "LastTime": 1446874989,
            "Replies": 1
        },
        {
            "ID": 3328,
            "Topic": "手机版和客户端版的贴内图片放大镜",
            "Tags": "建议",
            "UserID": 1738,
            "UserName": "simig",
            "LastName": "lincanbin",
            "LastTime": 1446814369,
            "Replies": 1
        },
        {
            "ID": 3327,
            "Topic": "【问题】为什么有些帖子的内容在评论里显示了。",
            "Tags": "帖子|显示|评论|内容",
            "UserID": 1543,
            "UserName": "过客。",
            "LastName": "lincanbin",
            "LastTime": 1446730727,
            "Replies": 2
        }
    ]
}
```

Fail:
* This API does not throw an error now. 
