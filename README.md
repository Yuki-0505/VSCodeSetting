# VSCodeSetting

# 1.1. 配置用户代码片段
> 文件 => 首选项 => 用户片段
```json
// Example:
"jQuery ajax": {
    "prefix": ".ajax",
    "body": [
        "$.ajax({",
        "\ttype: ${1|post,get,delete|},",
        "\turl: ${2:url},",
        "\tdata: ${3:data},",
        "\tdataType: ${4:json},",
        "\tsuccess: function (response) {",
        "\t\t$5",
        "\t}",
        "})"
    ],
    "description": "jQuery ajax"
}
```

# 2. 断点调试配置
> 点击左侧debug按钮 => 打开下拉栏，选择添加配置
```json
{
    "version": "0.2.0",
    "configurations": [
        {
            "type": "node",
            "request": "launch",
            "name": "Debug TypeScript",
            "runtimeArgs": ["-r", "ts-node/register"],
            "args": ["${workspaceFolder}/main.ts"]
        }
    ]
}
```
