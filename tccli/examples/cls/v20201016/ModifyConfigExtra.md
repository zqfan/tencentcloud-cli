**Example 1: 修改特殊采集配置任务**



Input: 

```
tccli cls ModifyConfigExtra --cli-unfold-argument  \
    --ConfigExtraId xxxx-xx-xx-xx-xxxxxxxx \
    --Name testname \
    --TopicId xxxxxx-xxx-xxxxxx \
    --Type host_file \
    --HostFile.LogPath /var/log/tmep \
    --HostFile.FilePattern *.log \
    --HostFile.CustomLabels key1=value1 key=value2 \
    --LogType minimalist_log \
    --ExtractRule.TimeKey date \
    --ExtractRule.TimeFormat %Y-%m-%d %H:%M:%S \
    --ExtractRule.Delimiter | \
    --ExtractRule.LogRegex .* \
    --ExtractRule.BeginRegex ^ \
    --ExtractRule.Keys date  content \
    --ExtractRule.FilterKeyRegex.0.Key xxx \
    --ExtractRule.FilterKeyRegex.0.Regex ssss \
    --ExtractRule.UnMatchLogKey testlog \
    --ExtractRule.UnMatchUpLoadSwitch True \
    --ExtractRule.Backtracking -1 \
    --ExcludePaths.0.Type xx \
    --ExcludePaths.0.Value xx \
    --UserDefineRule xxxxxx
```

Output: 
```
{
    "Response": {
        "RequestId": "6ef60bec-0242-43af-bb20-270359fb54a8"
    }
}
```

