**Example 1: 删除实例SQL限流任务**



Input: 

```
tccli dbbrain DeleteSqlFilters --cli-unfold-argument  \
    --InstanceId cdb-test \
    --SessionToken cAuth \
    --FilterIds 1234
```

Output: 
```
{
    "Response": {
        "RequestId": "24665720-8c93-11eb-bee6-e98cea0e6794"
    }
}
```

