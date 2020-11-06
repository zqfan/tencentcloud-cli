**Example 1: Creating the HAVIP**



Input: 

```
tccli vpc CreateHaVip --cli-unfold-argument  \
    --VpcId vpc-6v2ht8q5 \
    --SubnetId subnet-qq51iwr4 \
    --HaVipName test+name \
    --Vip 10.4.6.15
```

Output: 
```
{
    "Response": {
        "HaVip": {
            "HaVipId": "havip-72alakye",
            "HaVipName": "test name",
            "Vip": "10.4.6.15",
            "VpcId": "vpc-6v2ht8q5",
            "SubnetId": "subnet-qq51iwr4",
            "NetworkInterfaceId": "",
            "InstanceId": "",
            "AddressIp": "",
            "State": "UNBIND",
            "CreatedTime": "2018-10-10 17:03:09"
        },
        "RequestId": "fcb47621-838b-428e-8c33-6e210d93c451"
    }
}
```
