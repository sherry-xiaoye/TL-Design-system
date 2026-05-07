# Breadcrumb

## 使用场景

- 用于页面顶部展示当前位置层级，帮助用户返回上级页面。

## 允许变体

Default

## 尺寸与视觉

文字颜色使用文本 Token；间距、字号：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- current
- hover：待定

## 交互规则

- 位于 PageHeader 之前。
- 最后一级为当前页面，不可点击或点击无跳转。

## 前端适配

```tsx
<Breadcrumb items={[{ label: "首页" }, { label: "用户管理" }]} />
```

## 禁止事项

- 禁止把 Breadcrumb 做成按钮组。
- 禁止在层级中加入营销文案。

## AI 生成约束

- 必须优先调用系统 `Breadcrumb` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
