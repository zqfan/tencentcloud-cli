**Example 1: 获取标签歌曲**



Input: 

```
tccli yinsuda DescribeKTVMusicsByTag --cli-unfold-argument  \
    --UserId 20220123abc \
    --Limit 10 \
    --TagId 1111 \
    --AppName test
```

Output: 
```
{
    "Response": {
        "KTVMusicInfoSet": [
            {
                "AlbumInfo": {
                    "CoverInfoSet": [
                        {
                            "Dimension": "Mini",
                            "Url": "http://imge.xxxx.com/stdmusic/150/20191125/20191125163409414057.jpg"
                        },
                        {
                            "Dimension": "Small",
                            "Url": "http://imge.xxxx.com/stdmusic/240/20191125/20191125163409414057.jpg"
                        },
                        {
                            "Dimension": "Medium",
                            "Url": "http://imge.xxxx.com/stdmusic/480/20191125/20191125163409414057.jpg"
                        }
                    ],
                    "Name": "等"
                },
                "Duration": 216000,
                "MusicId": "mid-11x9dj3",
                "Name": "等",
                "SingerImageUrl": "http://singerimg.xxxxx.com/uploadpic/softhead/150/20210326/20210326145830248137.jpg",
                "SingerSet": [
                    "贾振峰"
                ],
                "RecommendType": "Other",
                "RightSet": [
                    "Play",
                    "Sing"
                ]
            }
        ],
        "RequestId": "58bfe77f-d477-48e8-9922-55f56d0b88fb",
        "ScrollToken": "eyJDdXJQYWdlTnVtIjozLCJDdXJJbmRleCI6MH0="
    }
}
```

