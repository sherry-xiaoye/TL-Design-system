# Dialog box

## 使用场景

- 用于确认、编辑、详情查看等模态流程。

## 允许变体

Confirm / Form / Detail（待定）

## 尺寸与视觉

背景使用 `--bms-color-bg-white`；宽度、圆角、内边距、遮罩：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- open
- closed
- loading
- error

## 交互规则

- 必须有明确标题。
- 确认类 Dialog 必须有主次按钮。
- 表单提交时确认按钮进入 loading。
- 高危操作必须使用 Confirm Dialog。

## 前端适配

```tsx
<Dialog open={open} title="确认删除" onConfirm={handleConfirm}>删除后不可恢复，是否继续？</Dialog>
```

## 禁止事项

- 禁止无标题弹窗。
- 禁止弹窗内再嵌套弹窗，除非业务确认。

## AI 生成约束

- 必须优先调用系统 `Dialog box` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
