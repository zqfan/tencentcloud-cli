**Example 1: 更新图片接口调用成功示例**



Input: 

```
tccli tiia UpdateImage --cli-unfold-argument  \
    --GroupId 123 \
    --EntityId 1 \
    --PicName test \
    --Tags 
```

Output: 
```
{
    "Response": {
        "RequestId": "cac925c7-c939-4e26-8db5-d642f7385c30"
    }
}
```

**Example 2: 更新图片接口调用失败示例**



Input: 

```
tccli tiia UpdateImage --cli-unfold-argument  \
    --GroupId  \
    --EntityId 1 \
    --PicName test
```

Output: 
```
{
    "Response": {
        "RequestId": "cac925c7-c939-4eb6-8db5-d64123385c30"
    }
}
```

