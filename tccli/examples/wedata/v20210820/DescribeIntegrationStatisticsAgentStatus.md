**Example 1: DescribeIntegrationStatisticsAgentStatus**



Input: 

```
tccli wedata DescribeIntegrationStatisticsAgentStatus --cli-unfold-argument  \
    --QueryDate 2022-01-01 \
    --TaskType 201 \
    --ProjectId 1 \
    --ExecutorGroupId 1
```

Output: 
```
{
    "Response": {
        "StatusData": "{\"running\":0}",
        "RequestId": "xx"
    }
}
```

