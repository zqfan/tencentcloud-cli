**Example 1: 升级后付费分布式DB**



Input: 

```
tccli dcdb UpgradeHourDCDBInstance --cli-unfold-argument  \
    --InstanceId dcdbt-fdpjf5zh \
    --UpgradeType ADD \
    --AddShardConfig.ShardCount 2 \
    --AddShardConfig.ShardMemory 2 \
    --AddShardConfig.ShardStorage 10
```

Output: 
```
{
    "Response": {
        "RequestId": "9b59ee51-0e13-1c2f-dedb-59fabe9d7f4a"
    }
}
```
