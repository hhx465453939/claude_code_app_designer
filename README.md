# Claude Code 项目架构模板

## 项目概述

这是一个专为Claude Code生态系统设计的标准化项目架构模板。该项目模板能够将抽象的项目需求转化为Claude Code可直接执行的完整项目结构，包含智能化的任务流程设计和上下文管理策略。

### 核心特性

- **架构思维导向**：从单个需求推导出完整的项目生态系统
- **Claude Code专家级集成**：深度理解MCP工具链和最佳实践
- **开箱即用**：标准化输出确保项目立即可用
- **策略预判机制**：主动识别技术难点并提供解决方案

## 快速开始

### 1. Claude Code 安装与配置

#### 安装Claude Code
1. 访问 [claude.ai/code](https://claude.ai/code) 下载最新版本
2. 按照官方指引完成安装
3. 确保系统已安装Node.js (v18+)

#### 基础配置
```bash
# 检查Claude Code版本
claude --version

# 配置全局设置
claude config set editor vscode
claude config set language zh-CN
```

### 2. 项目部署

#### 克隆项目模板
```bash
# 克隆项目到本地
git clone https://github.com/hhx465453939/claude_code_app_designer.git
# 修改文件夹名称为你的项目名：claude_code_app_template
cd claude_code_app_template

```

### 3. 核心文件说明

- **`Claude Code Project Architect.md`** - 主架构定义文件，包含系统提示词和项目生成逻辑
- **`CLAUDE.md`** - 项目指导文件，包含技术挑战解决方案
- **`README.md`** - 当前文件，部署和使用说明

## 使用指南

### 启动项目任务

#### 基础启动指令
```
请基于[项目需求描述]生成完整的Claude Code项目架构
```

#### 单一功能项目设计与自动化生成
```
# claude code会严格遵循规则生成项目结构与文件/脚本按照新应用逻辑更新README.md与CLAUDE.md，并删除原本的根目录文件;
# MCP工具选项二选一，代码使用选项二选一，原项目逻辑删除与否二选一

请严格遵守Claude_Code_Project_Architect.md与CLAUDE.md规定的规则，帮我创建一个用于实现<特定功能>的项目。

本项目<需要安装适配MCP工具>/<不需要安装任何新MCP工具>。
本项目<需要引入代码实现完整功能>/<不需要引入任何代码实现完整功能>。
首轮开发完成<删除>/<不删除>原CLAUDE.md，README.md与Claude_Code_Project_Architect.md，并更新本应用相关策略记忆文档CLAUDE.md与项目说明README.md
```

#### 多功能详细任务示例
```
# MCP工具选项二选一，代码使用选项二选一，原项目逻辑删除与否二选一

我需要一个电商数据分析平台的项目架构，包含：
- 数据采集模块
- 实时分析引擎  
- 可视化仪表板
- 用户权限管理
请生成完整的项目结构和必要的指令文件

本项目<需要安装适配MCP工具>/<不需要安装任何新MCP工具>。
本项目<需要引入代码实现完整功能>/<不需要引入任何代码实现完整功能>。
首轮开发完成<删除>/<不删除>原CLAUDE.md，README.md与Claude_Code_Project_Architect.md，并更新本应用相关策略记忆文档CLAUDE.md与项目说明README.md
```

### 任务调整与优化

#### 架构调整
```
请优化项目结构，增加缓存层和消息队列支持
```

#### 工具链配置
```
请配置Redis和Kafka相关的MCP工具集成
```

#### 性能优化
```
请分析当前架构的性能瓶颈并提供优化方案
```

### 自然语言指令模式

#### 1. 初始化检查指令
```
请检查当前项目状态并验证所有必要组件
```

#### 2. MCP工具配置指令
```
请配置数据库连接和API集成的MCP工具
```

#### 3. 任务执行指令
```
请执行数据模型生成任务，包含用户、订单、商品三个核心实体
```

#### 4. 问题排查指令
```
当前遇到上下文窗口限制，请提供分块处理策略
```

## 架构生成流程

### 标准执行流程
1. **需求解析** - 分析功能点、技术难点、依赖关系
2. **架构设计** - 生成目录结构和核心文件
3. **工具配置** - 设置必要的MCP工具
4. **质量验证** - 确保项目完整性和可执行性

### 输出组件
每次执行都会生成以下核心组件：
- 📁 完整的目录结构模板
- 📝 核心指令提示词文件
- 📋 部署使用说明文档
- 🧠 策略记忆文档

## 高级功能

### 上下文窗口管理
当处理大文件或复杂任务时：
```
请使用分块处理策略，将大型代码库分成多个可管理的片段
```

### MCP工具集成
支持的主要MCP工具：
- 数据库工具 (MySQL, PostgreSQL, MongoDB)
- API客户端工具
- 文件系统工具
- 版本控制工具

### 自定义扩展
```
请为项目添加自定义的AI辅助代码审查功能
```

## 故障排除

### 常见问题

#### Claude Code连接问题
```bash
# 重启Claude Code服务
claude restart

# 检查网络连接
claude ping
```

#### MCP工具配置错误
```
请重新验证MCP工具配置并提供详细错误信息
```

#### 上下文窗口超限
```
请使用摘要和分块策略处理大型文件
```

### 技术支持

如遇技术问题，请提供：
1. 错误日志内容
2. 当前项目状态
3. 执行的具体指令

## 项目结构(demo)

```
claude_code_app_template/
├── Claude Code Project Architect.md  # 主架构定义
├── CLAUDE.md                        # 项目指导文件  
├── README.md                        # 部署使用说明
├── package.json                     # 项目配置
├── src/                            # 源代码目录
│   ├── generators/                  # 生成器模块
│   ├── validators/                  # 验证器模块
│   └── utils/                      # 工具函数
└── templates/                      # 模板文件
    ├── project_structure/          # 项目结构模板
    ├── instructions/               # 指令模板
    └── documentation/              # 文档模板
```

## 版本更新

定期检查更新：
```bash
# 检查模板更新
npm run check-updates

# 更新到最新版本  
npm run update-template
```

## 贡献指南

欢迎提交Issue和Pull Request来改进这个模板项目。

## 许可证

MIT License - 详见LICENSE文件

---

**提示**：使用本项目模板时，请确保遵循Claude Code的最佳实践和安全指南。