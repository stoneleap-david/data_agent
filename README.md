# data_agent

## 使用 uv 安装依赖

### 1) 安装 uv

macOS:

```bash
brew install uv
```

或使用官方脚本:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

### 2) 进入项目目录

```bash
cd /Users/xudawei/Documents/AI/ai-project/data_agent
```

### 3) 按锁文件安装依赖（推荐）

```bash
uv sync
```

这会根据 `pyproject.toml` 和 `uv.lock` 创建并同步 `.venv`。

### 4) 常用命令

不手动激活虚拟环境，直接运行:

```bash
uv run python -V
uv run python -c "import fastapi, sqlalchemy; print('ok')"
```

如需手动激活:

```bash
source .venv/bin/activate
python -V
```

