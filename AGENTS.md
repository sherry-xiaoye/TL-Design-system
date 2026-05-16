# AGENTS.md

## Project

This repo contains Design System Markdown docs.

## Target structure

Keep this structure:

```text
TL_DesignSystem_Docs/
├── Guidelines/
├── Foundations/
├── Components/
├── Patterns/
├── README.md

## Source of truth

1. Figma link / Figma MCP
2. Existing tokens.json / tokens.css
3. Component screenshots
4. Existing Markdown docs

If a value is not confirmed by Figma or Token, mark it as `待定`.

Do not invent tokens.
Do not hardcode unverified size values.
Do not generate marketing-style UI rules.

## Component docs format

Every component document must use:

1. 使用场景
2. 允许变体
3. 尺寸与视觉
4. 状态
5. 交互规则
6. 前端适配
7. 禁止事项
8. AI 生成约束
