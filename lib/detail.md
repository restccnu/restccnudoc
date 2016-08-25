# 图书详情API

> 图书详情

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/lib/?id=xxxx&book=xxxx&author=xxxx&bid=xxxx | 无 | GET |

<hr/>

## URL Params

    id: 图书的id(可从图书搜索API中获取)
    book: 图书的名字
    author: 图书的作者
    bid: 图书索书号

## POST Data(json)

    无

## Return Data(json)

    {
        "bid": "xxxxx",  // 图书索书号
        "book": "xxxxxx",  // 图书名称
        "author": "xxxxxxx", // 图书作者
        "intro": "xxxxxx", // 图书介绍
        "books": [ // 该图书所有副本信息
            {
                "tid": "T112798172",  // 条码号
                "status": "可借/不可借/保留本",  // 借阅状态
                "room": "xxxxx",  // 馆藏地
                "date": "year-m-d" // 如果不可借, 显示归还日期
            },
            {....}
        ]
    }

## Status Code

    200 OK
    502 服务器端异常

## Notes
