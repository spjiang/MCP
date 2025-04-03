# MCP 客户端搭建流程

MCP开发要求借助uv进行虚拟环境创建和依赖管理。
uv 是一个Python 依赖管理工具，
类似于 pip 和 conda，但它更快、更高效，并且可以更好地管理 Python 虚拟环境和依赖项。
它的核心目标是替代 pip、venv 和 pip-tools，提供更好的性能和更低的管理开销。

## 创建 MCP 客户端项目
```bash
# 创建项目目录
uv init mcp-client
cd mcp-client
```

## 创建MCP客户端虚拟环境
uv会自动识别当前项目主目录并创建虚拟环境。
然后即可通过add方法在虚拟环境中安装相关的库。
```bash
# 创建虚拟环境
uv venv

# 激活虚拟环境
source .venv/bin/activate

```

## 安装 MCP SDK
```bash
# 安装 MCP SDK
uv add mcp
```

## 编写基础 MCP 客户端
- 创建client.py

##  运行 MCP 客户端
```bash
# 运行 MCP 客户端
uv run client.py
```

## MCP客户端接入OpenAI、DeepSeek在线模型流程
```bash
uv add mcp openai python-dotenv
```

## 创建.env文件
```bash
# 创建.env文件
touch .env
```

