**Example 1: DescribeIntegrationStatisticsInstanceTrend**



Input: 

```
tccli wedata DescribeIntegrationStatisticsInstanceTrend --cli-unfold-argument  \
    --QueryDate 2022-01-01 \
    --TaskType 201 \
    --ProjectId 1 \
    --ExecutorGroupId 1
```

Output: 
```
{
    "Response": {
        "TrendsData": [
            {
                "StatisticName": [
                    "a",
                    "b"
                ],
                "StatisticValue": [
                    2,
                    3
                ],
                "StatisticType": "typeA"
            }
        ],
        "RequestId": "xx"
    }
}
```

