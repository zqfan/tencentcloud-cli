**Example 1: 修改批次状态**



Input: 

```
tccli trp ModifyCodeBatch --cli-unfold-argument  \
    --BatchId xx \
    --Status 1
```

Output: 
```
{
    "Response": {
        "BatchId": "xx",
        "RequestId": "xx"
    }
}
```
