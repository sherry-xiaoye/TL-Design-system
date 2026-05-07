# BMS DesignSystem

本 DesignSystem 用于 BMS 后台管理系统设计规范、前端开发，以及 Cursor / Claude / Windsurf / Figma Make / Stitch 等 AI 工具协作。

## 结构

```text
DesignSystem/
├── Guidelines/        # 全局规则、AI Coding Rules、命名、自检清单
├── Foundations/       # 已确认 Token、颜色、字体、间距说明
├── Components/        # 组件实现契约
├── Patterns/          # 页面生成契约与示例
├── README.md
```

## 当前确认范围

- 已确认：颜色 Token，来源于 `Mode 1.tokens 2.json`。
- 待确认：组件高度、圆角、字号层级、行高、阴影、响应式断点。
- 原则：未经 Token 确认的尺寸，不得写死为 Token；文档中统一标注为“待定”。

## AI 使用方式

不要一次性把所有文档都塞给 AI。按页面类型加载，更稳定。

### 开发 TablePage 时读取

```text
Guidelines/AI_Coding_Rules.md
Guidelines/AI_Output_Checklist.md
Guidelines/Naming.md
Foundations/tokens.json
Foundations/tokens.css
Foundations/Color.md
Patterns/TablePage.md
Patterns/Examples/TablePage.example.md
Components/Button.md
Components/Input.md
Components/Select.md
Components/DatePicker.md
Components/Table.md
Components/Pagination.md
Components/Tooltip.md
Components/Loading.md
```

说明：Empty 先写入 Table / Pattern 的状态规则，是否独立为 `Components/Empty.md` 待确认。

### 开发 FormPage 时读取

```text
Guidelines/AI_Coding_Rules.md
Guidelines/AI_Output_Checklist.md
Guidelines/Naming.md
Foundations/tokens.json
Foundations/tokens.css
Foundations/Color.md
Patterns/FormPage.md
Patterns/Examples/FormPage.example.md
Components/Button.md
Components/Input.md
Components/Select.md
Components/DatePicker.md
Components/Radio.md
Components/Checkbox.md
Components/Switch.md
Components/Upload.md
Components/Dialog box.md
Components/Loading.md
```

### 开发 DetailPage 时读取

```text
Guidelines/AI_Coding_Rules.md
Guidelines/AI_Output_Checklist.md
Guidelines/Naming.md
Foundations/tokens.json
Foundations/tokens.css
Foundations/Color.md
Patterns/DetailPage.md
Components/Card.md
Components/Block Header.md
Components/Tag.md
Components/Table.md
Components/Button.md
Components/Loading.md
```

## 核心规则

1. 页面优先使用 `Patterns/` 中的页面生成契约。
2. 组件优先使用 `Components/` 中的系统组件契约。
3. 颜色只能使用 `Foundations/tokens.json` 或 `Foundations/tokens.css` 中的已确认颜色 Token。
4. 未确认尺寸标记为“待定”，不得伪造成 Token。
5. 禁止生成营销页、官网页、活动页、数据大屏风格。
