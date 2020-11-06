**Example 1: Describe Purge Tasks**



Input: 

```
tccli cdn DescribePurgeTasks --cli-unfold-argument  \
    --PurgeType url \
    --TaskId 1234567 \
    --Area mainland
```

Output: 
```
{
    "Response": {
        "RequestId": "4d5a83f8-a61f-445b-8036-5636be640bef",
        "PushLogs": [
            {
                "TaskId": "153303185323131331",
                "Url": "http://www.test.com/",
                "Status": "Done",
                "PurgeType": "url",
                "FlushType": "flush",
                "CreateTime": "2018-07-30 18:10:53"
            }
        ],
        "TotalCount": 1
    }
}
```
