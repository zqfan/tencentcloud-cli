**Example 1: Querying lifecycle hooks**



Input: 

```
tccli as DescribeLifecycleHooks --cli-unfold-argument ```

Output: 
```
{
    "Response": {
        "TotalCount": 4,
        "LifecycleHookSet": [
            {
                "LifecycleHookName": "terminate-topic",
                "AutoScalingGroupId": "asg-8fbozqja",
                "HeartbeatTimeout": 120,
                "NotificationMetadata": "topic",
                "NotificationTarget": {
                    "TargetType": "CMQ_TOPIC",
                    "TopicName": "one-topic",
                    "QueueName": ""
                },
                "CreatedTime": "2019-04-19T02:59:30Z",
                "DefaultResult": "ABANDON",
                "LifecycleHookId": "ash-oq76wsrx",
                "LifecycleTransition": "INSTANCE_TERMINATING"
            },
            {
                "LifecycleHookName": "launch-queue",
                "AutoScalingGroupId": "asg-8fbozqja",
                "HeartbeatTimeout": 120,
                "NotificationMetadata": "queue",
                "NotificationTarget": {
                    "TargetType": "CMQ_QUEUE",
                    "TopicName": "",
                    "QueueName": "one-queue"
                },
                "CreatedTime": "2019-04-19T02:57:14Z",
                "DefaultResult": "CONTINUE",
                "LifecycleHookId": "ash-fbjiexz7",
                "LifecycleTransition": "INSTANCE_LAUNCHING"
            },
            {
                "LifecycleHookName": "one-hook",
                "AutoScalingGroupId": "asg-8fbozqja",
                "HeartbeatTimeout": 360,
                "NotificationMetadata": "",
                "NotificationTarget": {
                    "TargetType": "",
                    "TopicName": "",
                    "QueueName": ""
                },
                "CreatedTime": "2019-04-19T02:56:02Z",
                "DefaultResult": "CONTINUE",
                "LifecycleHookId": "ash-heyubibl",
                "LifecycleTransition": "INSTANCE_LAUNCHING"
            },
            {
                "LifecycleHookName": "one-hook-default",
                "AutoScalingGroupId": "asg-8fbozqja",
                "HeartbeatTimeout": 300,
                "NotificationMetadata": "",
                "NotificationTarget": {
                    "TargetType": "",
                    "TopicName": "",
                    "QueueName": ""
                },
                "CreatedTime": "2019-04-19T02:51:24Z",
                "DefaultResult": "CONTINUE",
                "LifecycleHookId": "ash-8azjzxj9",
                "LifecycleTransition": "INSTANCE_LAUNCHING"
            }
        ],
        "RequestId": "dff07f6e-bdbc-4532-baeb-e7fb3aebe248"
    }
}
```

**Example 2: Using Filter to query lifecycle hooks**



Input: 

```
tccli as DescribeLifecycleHooks --cli-unfold-argument  \
    --Filters.0.Name lifecycle-hook-id \
    --Filters.0.Values ash-oq76wsrx ash-fbjiexz7 \
    --Filters.1.Name auto-scaling-group-id \
    --Filters.1.Values asg-8fbozqja
```

Output: 
```
{
    "Response": {
        "TotalCount": 2,
        "LifecycleHookSet": [
            {
                "LifecycleHookName": "terminate-topic",
                "AutoScalingGroupId": "asg-8fbozqja",
                "HeartbeatTimeout": 120,
                "NotificationMetadata": "topic",
                "NotificationTarget": {
                    "TargetType": "CMQ_TOPIC",
                    "TopicName": "one-topic",
                    "QueueName": ""
                },
                "CreatedTime": "2019-04-19T02:59:30Z",
                "DefaultResult": "ABANDON",
                "LifecycleHookId": "ash-oq76wsrx",
                "LifecycleTransition": "INSTANCE_TERMINATING"
            },
            {
                "LifecycleHookName": "launch-queue",
                "AutoScalingGroupId": "asg-8fbozqja",
                "HeartbeatTimeout": 120,
                "NotificationMetadata": "queue",
                "NotificationTarget": {
                    "TargetType": "CMQ_QUEUE",
                    "TopicName": "",
                    "QueueName": "one-queue"
                },
                "CreatedTime": "2019-04-19T02:57:14Z",
                "DefaultResult": "CONTINUE",
                "LifecycleHookId": "ash-fbjiexz7",
                "LifecycleTransition": "INSTANCE_LAUNCHING"
            }
        ],
        "RequestId": "2d774a6c-bcaa-4805-b0cd-bd64519e2538"
    }
}
```
