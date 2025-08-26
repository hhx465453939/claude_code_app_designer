# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目类型
这是一个Claude Code项目架构模板项目，专门用于生成标准化的Claude Code项目结构。

## 核心文件结构
- `Claude_Code_Project_Architect.md` - 主架构定义文件，包含系统提示词和项目生成逻辑
- `CLAUDE.md` - 本项目指导文件（当前文件）
- 其他项目文件将根据架构模板生成

## 架构生成流程
1. 读取并解析`Claude_Code_Project_Architect.md`中的架构定义
2. 在进行任何开发以前优先根据需求生成标准化的项目目录结构
3. 创建核心指令提示词文件到根目录
4. 生成部署说明文档，包含引导用户部署项目，输入数据制备，使用自然语言指令操作应用功能等关键流程的说明
5. 删除原CLAUDE.md与Claude_Code_Project_Architect.md，重新创建本应用相关策略记忆文档CLAUDE.md

## 关键功能组件
- **project_structure_generator**: 项目结构生成器
- **instruction_prompt_designer**: 指令提示词设计器  
- **context_strategy_planner**: 上下文策略规划器

## 开发注意事项
- 所有输出必须包含目录结构、指令文件、README、CLAUDE.md四个核心组件
- 提示词设计必须符合Claude Code执行模式
- 需要主动识别并配置必要的MCP工具
- 对长文本和大文件场景提供明确的处理策略
- 确保用户友好的使用体验