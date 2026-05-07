# Switch

## 使用场景

- 用于即时启用 / 停用状态。

## 允许变体

Default

## 尺寸与视觉

开启色优先使用品牌色 Token；尺寸、圆角：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- off
- on
- disabled
- loading

## 交互规则

- 触发服务端状态变更时必须显示 loading 或禁用。
- 高风险开关需二次确认。

## 前端适配

```tsx
<Switch checked={enabled} loading={loading} />
```

## 禁止事项

- 禁止把 Switch 用于需要提交表单后生效的普通字段，除非业务确认。

## AI 生成约束

- 必须优先调用系统 `Switch` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
