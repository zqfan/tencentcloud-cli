**Example 1: 获取Session Statement详情列表**

本接口用于获取Session Statement详情列表。

Input: 

```
tccli dlc DescribeNotebookSessionStatements --cli-unfold-argument  \
    --SessionId d3018ad4-9a7e-4f64-a3f4-f38507c69742 \
    --BatchId eiosldd7-ekd4-4e5e-993e-e5db64fa21c1
```

Output: 
```
{
    "Response": {
        "NotebookSessionStatements": {
            "NotebookSessionStatementBatch": [
                {
                    "Completed": 0,
                    "Started": 0,
                    "Progress": 0,
                    "StatementId": "ksiked7-ekd4-4e5e-993e-e5db64fa21c1",
                    "TaskId": "d301fsdd4-9a7e-4f64-a3dj-f38507c697dj",
                    "State": "available",
                    "OutPut": {
                        "ExecutionCount": 0,
                        "Data": [
                            {
                                "Key": "testKey",
                                "Value": "testValue"
                            }
                        ],
                        "Status": "available",
                        "ErrorName": "testErrorName",
                        "ErrorValue": "testErrorValue",
                        "ErrorMessage": [
                            "testErrorMessage"
                        ],
                        "SQLResult": "result"
                    },
                    "BatchId": "eiosldd7-ekd4-4e5e-993e-e5db64fa21c1"
                }
            ],
            "IsAvailable": true,
            "SessionId": "ksjeldd7-ekd4-4e5e-993e-e5db64fa21c1"
        },
        "RequestId": "b8sd7dd7-ekd4-4e5e-993e-e5db64fa21c1"
    }
}
```

