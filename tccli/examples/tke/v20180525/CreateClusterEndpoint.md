**Example 1: 创建集群访问端口**



Input: 

```
tccli tke CreateClusterEndpoint --cli-unfold-argument  \
    --SubnetId subnet-xxxxxx \
    --ClusterId cls-xxxxxxxx
```

Output: 
```
{
    "Response": {
        "RequestId": "eac6b301-a322-493a-8e36-83b295459397"
    }
}
```

