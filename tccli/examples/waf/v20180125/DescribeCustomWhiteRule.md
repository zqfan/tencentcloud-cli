**Example 1: 获取精准白名单规则列表**



Input: 

```
tccli waf DescribeCustomWhiteRule --cli-unfold-argument  \
    --Domain test.qcloudwaf.com \
    --Limit 1 \
    --Filters.0.Values 1234567890 \
    --Filters.0.Name RuleID \
    --Filters.0.ExactMatch True \
    --Offset 1
```

Output: 
```
{
    "Response": {
        "RequestId": "5d207f4f-0d41-4f5d-bce2-0320090c98d8",
        "RuleList": [
            {
                "ActionType": "1",
                "Bypass": "geoip,cc,owasp,ai,antileakage",
                "CreateTime": "2020-02-20 14:00:12",
                "ExpireTime": "0",
                "Name": "test",
                "Redirect": "/",
                "RuleId": "17958569",
                "SortId": "100",
                "Status": "1",
                "Strategies": [
                    {
                        "Arg": "",
                        "CompareFunc": "ipmatch",
                        "Content": "1.1.1.2",
                        "Field": "IP"
                    }
                ]
            }
        ],
        "TotalCount": "1"
    }
}
```
