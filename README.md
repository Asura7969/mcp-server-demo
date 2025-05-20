# mcp-simple-resource

引用：[mcp-simple-resource](https://github.com/modelcontextprotocol/python-sdk/blob/main/examples/servers/simple-resource/README.md)

python环境3.12.0

### MCP Server
## 环境配置
* 安装`uv`: https://docs.astral.sh/uv/
* uv sync

> 设置阿里云镜像(全局)
> UV_DEFAULT_INDEX=https://mirrors.aliyun.com/pypi/simple/


```shell
# 运行
uv run mcp-simple-resource --transport sse --port 8000
```

### MCP Host
`cline mcp config`
```json
{
    "mcpServers": {
        "mcp-simple-resource": {
            "url": "http://127.0.0.1:8000/sse",
            "disabled": false,
            "autoApprove": []
        }
    }
}
```