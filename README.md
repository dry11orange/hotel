# hotel

## GitHub Copilot 编码代理能做什么操作？/ What can the Copilot coding agent do?

GitHub Copilot 编码代理（Coding Agent）可以在这个仓库中执行以下操作：

### 代码操作 / Code Operations
- **读取和理解代码**：浏览、搜索和分析仓库中的文件与代码
- **创建新文件**：在仓库中新建文件（源代码、配置、文档等）
- **编辑现有文件**：修改已有文件的内容
- **重构代码**：在现有代码基础上进行改进和重构

### 开发工作流 / Development Workflow
- **运行构建和测试**：执行仓库中已有的构建脚本、测试套件和代码检查工具
- **安装依赖**：通过包管理器（npm、pip、go 等）安装所需依赖
- **执行 Shell 命令**：在沙盒环境中运行 bash 命令

### GitHub 集成 / GitHub Integration
- **查看 Issues 和 Pull Requests**：读取 GitHub Issues、PR 详情、评论等
- **查看工作流运行结果**：检查 GitHub Actions 的运行状态和日志
- **提交代码变更**：通过 PR 将代码变更推送到 GitHub

### 信息检索 / Information Retrieval
- **搜索代码**：在仓库及 GitHub 上搜索代码、文件和符号
- **获取文件内容**：读取仓库中任意文件的内容
- **访问网页**：获取公开网页上的信息（部分域名受限）

### 安全扫描 / Security Scanning
- **代码安全检查**：使用 CodeQL 扫描代码中的安全漏洞
- **依赖漏洞检查**：检查依赖项是否存在已知安全漏洞

### 限制 / Limitations
代理**不能**执行以下操作：
- 直接使用 `git push` 或 `gh` 命令提交代码（必须通过 `report_progress` 工具）
- 访问或修改其他仓库
- 创建新的 Issue 或 PR
- 强制推送或变基提交历史
- 访问 `.github/agents` 目录中的文件