**Example 1: 1分钟内，CPU平均利用率大于50%，连续发生5次，期望实例数增加1**



Input: 

```
tccli as CreateScalingPolicy --cli-unfold-argument  \
    --AutoScalingGroupId asg-12wjuh0s \
    --Cooldown 60 \
    --ScalingPolicyName cpu_policy_test \
    --AdjustmentType  CHANGE_IN_CAPACITY \
    --MetricAlarm.Period 60 \
    --MetricAlarm.ContinuousTime 5 \
    --MetricAlarm.ComparisonOperator GREATER_THAN \
    --MetricAlarm.Statistic AVERAGE \
    --MetricAlarm.Threshold 50 \
    --MetricAlarm.MetricName CPU_UTILIZATION \
    --NotificationUserGroupIds 1678 \
    --AdjustmentValue 1
```

Output: 
```
{
    "Response": {
        "AutoScalingPolicyId": "asp-iir70sxv",
        "RequestId": "fb02c8bd-5f38-4786-91b6-0c6e06a88832"
    }
}
```

**Example 2: 1分钟内，内存平均利用率小于35%，连续发生5次，减少50%实例**



Input: 

```
tccli as CreateScalingPolicy --cli-unfold-argument  \
    --AutoScalingGroupId asg-12wjuh0s \
    --Cooldown 300 \
    --ScalingPolicyName mem_policy_test \
    --AdjustmentType  PERCENT_CHANGE_IN_CAPACITY \
    --MetricAlarm.Period 60 \
    --MetricAlarm.ContinuousTime 5 \
    --MetricAlarm.ComparisonOperator LESS_THAN \
    --MetricAlarm.Statistic AVERAGE \
    --MetricAlarm.Threshold 50 \
    --MetricAlarm.MetricName MEM_UTILIZATION \
    --NotificationUserGroupIds 1678 \
    --AdjustmentValue -50
```

Output: 
```
{
    "Response": {
        "AutoScalingPolicyId": "asp-f59pppuh",
        "RequestId": "116213d6-2269-44cc-af76-c4a8dc7dbdf9"
    }
}
```

