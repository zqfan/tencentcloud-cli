**Example 1: Getting the first two lists of basic policy alarm groups**



Input: 

```
tccli monitor DescribePolicyGroupList --cli-unfold-argument  \
    --Module monitor \
    --Limit 2 \
    --Offset 0
```

Output: 
```
{
    "Response": {
        "GroupList": [
            {
                "CanSetDefault": true,
                "Conditions": [
                    {
                        "AlarmNotifyPeriod": 86400,
                        "AlarmNotifyType": 0,
                        "CalcType": 1,
                        "CalcValue": "0",
                        "ContinueTime": 60,
                        "MetricId": 33,
                        "MetricShowName": "CPU usage",
                        "Period": 60,
                        "RuleId": 1111111,
                        "Unit": "%"
                    }
                ],
                "ConditionsTemp": null,
                "EventConditions": [
                    {
                        "AlarmNotifyPeriod": 0,
                        "AlarmNotifyType": 0,
                        "EventId": 42,
                        "EventShowName": "ping unreachable",
                        "RuleId": 1111112
                    }
                ],
                "GroupId": 1111111,
                "GroupName": "Copying-test",
                "InsertTime": 1531122504,
                "InstanceGroup": null,
                "IsDefault": 0,
                "IsOpen": true,
                "LastEditUin": "1500000000",
                "NoShieldedSum": 0,
                "ParentGroupId": 0,
                "ProjectId": 0,
                "ReceiverInfos": [
                    {
                        "EndTime": 86400,
                        "NeedSendNotice": 1,
                        "NotifyWay": [
                            "EMAIL",
                            "SMS"
                        ],
                        "PersonInterval": 60,
                        "ReceiverGroupList": [
                            1111
                        ],
                        "ReceiverType": "group",
                        "ReceiverUserList": [],
                        "RecoverNotify": [
                            "SMS"
                        ],
                        "RoundInterval": 60,
                        "RoundNumber": 2,
                        "SendFor": [],
                        "StartTime": 0,
                        "UidList": null
                    }
                ],
                "Remark": "",
                "UpdateTime": 1577689096,
                "UseSum": 0,
                "ViewName": "cvm_device"
            },
            {
                "CanSetDefault": false,
                "Conditions": [
                    {
                        "AlarmNotifyPeriod": 0,
                        "AlarmNotifyType": 0,
                        "CalcType": 1,
                        "CalcValue": "0.85",
                        "ContinueTime": 300,
                        "MetricId": 1220,
                        "MetricShowName": "Disk usage",
                        "Period": 60,
                        "RuleId": 1111113,
                        "Unit": ""
                    }
                ],
                "ConditionsTemp": null,
                "EventConditions": null,
                "GroupId": 1111112,
                "GroupName": "Default",
                "InsertTime": 1565792922,
                "InstanceGroup": null,
                "IsDefault": 1,
                "IsOpen": true,
                "LastEditUin": "1500000687",
                "NoShieldedSum": 1,
                "ParentGroupId": 0,
                "ProjectId": 0,
                "ReceiverInfos": null,
                "Remark": "",
                "UpdateTime": 1565792922,
                "UseSum": 1,
                "ViewName": "CKAFKA_INSTANCE"
            }
        ],
        "RequestId": "5fdf1257-6024-4b59-b924-2b995080f0bd",
        "Total": 142
    }
}
```
