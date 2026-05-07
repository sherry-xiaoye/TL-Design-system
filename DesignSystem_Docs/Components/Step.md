# Step

## 使用场景

- 用于流程步骤展示，例如创建流程、审批流程、配置向导。

## 允许变体

Horizontal / Vertical（待定）

## 尺寸与视觉

完成态可使用成功色 Token；当前态可使用品牌色 Token；尺寸待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- wait
- process
- finish
- error
- disabled：待定

## 交互规则

- 步骤文案保持简短。
- 当前步骤必须清晰可见。

## 前端适配

```tsx
<Steps current={current} items={items} />
```

## 禁止事项

- 禁止把 Step 用作普通导航。

## AI 生成约束

- 必须优先调用系统 `Step` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
