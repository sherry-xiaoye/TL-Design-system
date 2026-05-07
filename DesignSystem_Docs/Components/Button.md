# Button

## 使用场景

- Primary：页面主操作，例如“新增”“保存”“查询”。
- Default：次要操作，例如“取消”“重置”。
- Text：表格行内操作，例如“查看”“编辑”“删除”。
- Danger：高危操作，例如“删除”“作废”“停用”。

## 允许变体

Primary / Default / Text / Danger

## 尺寸与视觉

Primary 使用 `--bms-color-brand`；Default 背景使用 `--bms-color-bg-white`；边框优先使用 `--bms-color-border-table-line`。高度、内边距、圆角：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- hover：待定
- active：待定
- disabled：文字使用禁用文本 Token，背景/边框待定
- loading：异步提交必须出现

## 交互规则

- 异步提交时按钮进入 loading。
- 高危操作必须二次确认。
- 表格行内操作优先使用 Text Button。
- 同一区域不建议多个 Primary Button 并列。

## 前端适配

```tsx
<Button type="primary">查询</Button>
<Button>重置</Button>
<Button type="text">编辑</Button>
<Button danger>删除</Button>
```

## 禁止事项

- 禁止用 div / span 模拟按钮。
- 禁止自定义按钮颜色。
- 禁止在表格操作列使用大尺寸 Primary 按钮。

## AI 生成约束

- 必须优先调用系统 `Button` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
