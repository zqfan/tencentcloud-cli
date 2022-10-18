**Example 1: 创建应用代理规则**



Input: 

```
tccli teo CreateApplicationProxyRule --cli-unfold-argument  \
    --ZoneId zone-21xfqlh4qjee \
    --ProxyId proxy-19389e5dwwxfs \
    --Proto TCP \
    --Port 80 90 99-110 \
    --OriginType custom \
    --OriginValue 1.1.1.1:80 \
    --ForwardClientIp TOA \
    --SessionPersist False
```

Output: 
```
{
    "Response": {
        "RequestId": "3df3e931-3159-4337-adc7-7604e01e0fa9",
        "RuleId": "rule-a8f0d49a-33d7-11ed-9b89-52540005c111"
    }
}
```
