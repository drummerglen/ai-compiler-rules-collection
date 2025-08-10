# AI编译器 Rules 合集

一个面向 AI 编程工具（Trae、Cursor、Claude、Copilot 等）的规则与工作流模板合集，帮助你以“文档先行、任务递归、范围收敛”的方式实现可控交付。

当前已收录：
- 6A 工作流规则模板（6A.md）：完整的六阶段工作流，覆盖 Align → Architect → Atomize → Approve → Automate → Assess 全流程。

## 仓库定位
- 面向个人/团队沉淀统一的规则集（Rules as Code）
- 让不同 AI 工具共享一套规范与流程
- 支持持续扩展：后续可按规则类型添加更多 rules

## 目录结构（建议）
- 根目录
  - 6A.md：6A 工作流规则模板（已加入）
  - rules/：可新增其它规则（如编码规范、CR检查清单、架构模板等）
  - README.md：本说明文档

可选扩展（后续需要时再添加）：
- rules/architecture/ 体系化架构规则
- rules/review/ Code Review 检查清单
- rules/testing/ 测试策略与覆盖要求
- rules/security/ 安全规范与密钥管理

## 使用方式
1) 直接复制根目录的 6A.md 到你的 AI 工具（Trae/ Cursor 等）作为自定义规则/工作流
2) 或将 6A.md 内容合并到工具的规则系统（例如 Trae 的自定义规则、Cursor 的 .cursorrules）
3) 按 6A 流程执行时，建议逐阶段产出相应文档（ALIGNMENT/CONSENSUS/DESIGN/TASK/ACCEPTANCE/FINAL/TODO）

注意：
- 若你需要在 Trae 中固化规则，请手动将内容配置到 Trae 的规则系统；由于我无法直接访问你本地的 Trae 配置文件（如 mcp.json），需你手动更新后再继续操作。

## 如何新增更多 Rules（后续）
- 在 rules/ 下按主题或工具创建子文件夹，例如：
  - rules/architecture/
  - rules/review/
  - rules/testing/
  - rules/security/
- 每个规则文件以 Markdown 方式撰写，包含：规则目标、适用范围、执行步骤、验收标准、质量门控等
- 如为复杂工作流，推荐包含：流程图（Mermaid）、输入输出规范、错误处理策略等

## 版权与声明
- 规则内容支持在团队内部使用并二次定制
- 若对外发布，请保留来源说明

——
欢迎持续补充更多规则，我们将把本仓库作为“AI 编译器 rules 合集”的统一入口与沉淀地。