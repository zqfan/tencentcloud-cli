**Example 1: 容器网络创建网络策略添加并发布任务务示例**



Input: 

```
tccli tcss AddAndPublishNetworkFirewallPolicyDetail --cli-unfold-argument  \
    --PolicyName xx \
    --CustomPolicy.0.Peer xx \
    --CustomPolicy.0.Direction xx \
    --CustomPolicy.0.Ports xx \
    --Description xx \
    --ClusterId xx \
    --FromPolicyRule 0 \
    --Namespace xx \
    --ToPolicyRule 0 \
    --PodSelector xx
```

Output: 
```
{
    "Response": {
        "RequestId": "345da107-dfdf-48f0-9796-e6723bdc102e",
        "TaskId": 32501,
        "Result": "Succ"
    }
}
```

