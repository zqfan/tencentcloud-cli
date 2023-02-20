**Example 1: 新建全局告警通知渠道**

新建全局告警通知渠道

Input: 

```
tccli monitor CreatePrometheusGlobalNotification --cli-unfold-argument  \
    --InstanceId xx \
    --Notification.AlertManager.Url xx \
    --Notification.AlertManager.ClusterId xx \
    --Notification.AlertManager.ClusterType xx \
    --Notification.RepeatInterval xx \
    --Notification.WebHook xx \
    --Notification.Enabled True \
    --Notification.PhoneNotifyOrder 1 \
    --Notification.PhoneInnerInterval 0 \
    --Notification.PhoneCircleInterval 0 \
    --Notification.NotifyWay xx \
    --Notification.ReceiverGroups xx \
    --Notification.PhoneArriveNotice True \
    --Notification.PhoneCircleTimes 0 \
    --Notification.TimeRangeStart xx \
    --Notification.Type xx \
    --Notification.TimeRangeEnd xx
```

Output: 
```
{
    "Response": {
        "Id": "xx",
        "RequestId": "xx"
    }
}
```
