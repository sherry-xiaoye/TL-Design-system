# Pagination

## 使用场景

- 用于表格或列表分页。

## 允许变体

Default

## 尺寸与视觉

尺寸、间距：待定；激活态优先使用品牌色 Token。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- active
- disabled

## 交互规则

- 位于表格下方，通常右对齐。
- 数据量为 0 时不展示分页。
- 是否包含每页条数选择按业务待定。

## 前端适配

```tsx
<Pagination current={page} pageSize={pageSize} total={total} />
```

## 禁止事项

- 禁止数据为 0 时仍展示分页。
- 禁止分页位置随页面变化。

## AI 生成约束

- 必须优先调用系统 `Pagination` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
