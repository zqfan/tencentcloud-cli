**Example 1: 修改负载均衡实例名称**



Input: 

```
tccli clb ModifyLoadBalancerAttributes --cli-unfold-argument  \
    --LoadBalancerName newlbname \
    --LoadBalancerId lb-6efswuxa
```

Output: 
```
{
    "Response": {
        "DealName": null,
        "RequestId": "78a40898-8210-44c7-8bc6-f83e50878d12"
    }
}
```

**Example 2: 设置负载均衡实例的跨域属性**



Input: 

```
tccli clb ModifyLoadBalancerAttributes --cli-unfold-argument  \
    --TargetRegionInfo.Region ap-shanghai \
    --TargetRegionInfo.VpcId vpc-abcd1234 \
    --LoadBalancerId lb-6efswuxa
```

Output: 
```
{
    "Response": {
        "DealName": null,
        "RequestId": "78a40898-8210-44c7-8bc6-f83e5087ad54"
    }
}
```

