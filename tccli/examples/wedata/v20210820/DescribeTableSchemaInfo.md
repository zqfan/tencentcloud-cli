**Example 1: 获取表schema信息**



Input: 

```
tccli wedata DescribeTableSchemaInfo --cli-unfold-argument  \
    --MsType HIVE \
    --Name 字符串 \
    --DatabaseName 字符串 \
    --DatasourceId 23432 \
    --ConnectionType rpc
```

Output: 
```
{
    "Response": {
        "SchemaInfoList": [
            {
                "ColumnKey": "xx",
                "Type": "xx",
                "Description": "xx",
                "Name": "xx"
            }
        ],
        "RequestId": "xx"
    }
}
```

