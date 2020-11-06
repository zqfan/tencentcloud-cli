**Example 1: Deleting layer-4 forwarding rules**



Input: 

```
tccli dayu DeleteL4Rules --cli-unfold-argument  \
    --Business bgpip \
    --Id bgpip-000000xd \
    --RuleIdList rule-00000001
```

Output: 
```
{
    "Response": {
        "RequestId": "eac6b301-a322-493a-8e36-83b295459397",
        "Success": {
            "Code": "Success",
            "Message": "Success"
        }
    }
}
```
