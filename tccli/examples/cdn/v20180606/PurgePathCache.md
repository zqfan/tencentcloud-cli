**Example 1: Submitting a directory purge task**



Input: 

```
tccli cdn PurgePathCache --cli-unfold-argument  \
    --Paths http://www.test.com/test/ \
    --FlushType flush
```

Output: 
```
{
    "Response": {
        "RequestId": "4d5a83f8-a61f-445b-8036-5636be640bef",
        "TaskId": "1533045796-i60rfmzm"
    }
}
```
