**Example 1: Querying the list of parameter templates**



Input: 

```
tccli cdb DescribeParamTemplates --cli-unfold-argument ```

Output: 
```
{
    "Response": {
        "RequestId": "756bb037-a44a-4b4f-abe0-6efd34a6c792",
        "TotalCount": 1,
        "Items": [
            {
                "TemplateId": 2333,
                "Name": "test",
                "Description": "test",
                "EngineVersion": "5.7"
            }
        ]
    }
}
```
