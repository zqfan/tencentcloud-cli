**Example 1: 禁用SSL-VPN-CLIENT证书**



Input: 

```
tccli vpc DisableVpnGatewaySslClientCert --cli-unfold-argument  \
    --SslVpnClientId vpnc-xxxx
```

Output: 
```
{
    "Response": {
        "RequestId": "aeabeab6-f74b-453a-b25d-d7b460193c3b",
        "TaskId": 123
    }
}
```

