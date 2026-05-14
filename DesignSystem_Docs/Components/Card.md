# Card

## 1.1 用途

用于承载相对独立的信息块，例如仪表盘指标、详情分组、列表卡片。

## 1.2 视觉规范

- 组件：`Card`
- State：`Default`, `Hover`
- 颜色：优先使用 Semantic Token，其次 Primitive Token，禁止自定义色值
- 尺寸：待定
- 内边距：待定
- 圆角：待定
- 边框 / 阴影：待定
- 字体：待定

## 1.3 状态规范

- default：`Default`
- hover：`Hover`
- active / focus：待定
- blur：待定
- disabled：待定
- error：待定
- loading：待定

## 1.4 交互规则

- Card 可用于展示内容分组。
- 仅在 Figma 或业务明确时作为可点击卡片。
- 禁止卡片嵌套卡片。

## 1.5 业务场景示例

- 场景 1：【仪表盘业务】中的【指标卡片】
- 场景 2：【详情业务】中的【信息分组】

## 1.6 前端适配点

- `state` 映射 `Default | Hover`
- `title` / `content` / `actions` 结构待定
- 组件名建议：`Card`

## 1.7 AI 生成约束

- 必须使用系统 `Card`。
- 禁止将页面大区块全部做成浮动卡片。
- 禁止卡片套卡片。
- 禁止新增未在 Figma 出现的尺寸、颜色、状态、圆角、阴影。
