**Example 1: Creating a monthly subscription TencentDB instance**



Input: 

```
tccli mongodb CreateDBInstance --cli-unfold-argument  \
    --Memory 4 \
    --Volume 250 \
    --GoodsNum 1 \
    --Zone ap-guangzhou-2 \
    --UniqVpcId vpc-0akbol5v \
    --UniqSubnetId subnet-fyrtjbqw \
    --ProjectId 0 \
    --MongoVersion MONGO_3_WT \
    --MachineCode TGIO \
    --NodeNum 3 \
    --Period 1 \
    --Password pwd123456 \
    --ClusterType REPLSET \
    --ReplicateSetNum 1
```

Output: 
```
{
    "Response": {
        "RequestId": "d88095e5-50e8-4245-a0cf-993a536f9b20",
        "DealId": "7142863",
        "InstanceIds": [
            "cmgo-po5f899l"
        ]
    }
}
```
