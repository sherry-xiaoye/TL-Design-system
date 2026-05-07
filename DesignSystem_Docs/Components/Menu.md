# Menu

## 使用场景

- 用于左侧导航。

## 允许变体

Default / Collapsed（待定）

## 尺寸与视觉

背景使用 `--bms-color-bg-menu`；选中态颜色待定，优先使用品牌色 Token。宽度、行高、缩进：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- active
- hover：待定
- disabled

## 交互规则

- 菜单项文案保持简短。
- 最多建议三级层级，超过需重构信息架构。

## 前端适配

```tsx
<Menu items={menuItems} selectedKeys={selectedKeys} />
```

## 禁止事项

- 禁止在菜单中放置广告、营销模块。
- 禁止多套菜单样式混用。

## AI 生成约束

- 必须优先调用系统 `Menu` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
