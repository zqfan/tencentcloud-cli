**Example 1: 创建spark应用**

本接口用于创建spark应用。

Input: 

```
tccli dlc ModifySparkApp --cli-unfold-argument  \
    --SparkAppId batch_sadfafd \
    --AppName spark-test \
    --AppType 1 \
    --DataEngine spark-engine \
    --Eni kafka-eni \
    --IsLocal cos \
    --AppFile test.jar \
    --RoleArn 12 \
    --MainClass com.test.WordCount \
    --AppConf spark-default.properties \
    --IsLocalJars cos \
    --AppJars com.test2.jar \
    --IsLocalFiles cos \
    --AppFiles spark-default.properties \
    --AppDriverSize small \
    --AppExecutorSize small \
    --AppExecutorNums 1 \
    --AppExecutorMaxNumbers 1
```

Output: 
```
{
    "Response": {
        "RequestId": "2ae4707a-9f72-44aa-9fd4-65cb739d6301"
    }
}
```

