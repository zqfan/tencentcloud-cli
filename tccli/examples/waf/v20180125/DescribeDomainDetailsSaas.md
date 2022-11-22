**Example 1: 查询单个saas域名详情**



Input: 

```
tccli waf DescribeDomainDetailsSaas --cli-unfold-argument  \
    --Domain lucasssli3.qcloud.com \
    --DomainId 20200728142847163546341 \
    --InstanceId waf_000000002
```

Output: 
```
{
    "Response": {
        "RequestId": "b4f13899-561b-46a0-a045-6ba6b72c38f2",
        "DomainsPartInfo": {
            "CertType": 0,
            "Cls": 0,
            "Cname": "",
            "HttpsRewrite": 0,
            "HttpsUpstreamPort": "",
            "IsKeepAlive": 0,
            "IsCdn": 0,
            "IsGray": 0,
            "IsHttp2": 0,
            "IsWebsocket": 0,
            "LoadBalance": 0,
            "Mode": 0,
            "PrivateKey": "",
            "SSLId": "",
            "UpstreamDomain": "",
            "UpstreamScheme": "",
            "UpstreamType": 0,
            "SrcList": [],
            "Ports": [],
            "ActiveCheck": 1
        }
    }
}
```
