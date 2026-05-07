# Naming

命名规则必须区分 Figma 组件变体、代码组件使用方式、CSS class，不得混用。

## 1. Figma 组件变体命名

使用 PascalCase + 中横线：

```text
Button-Primary-Default
Button-Primary-Hover
Button-Danger-Small-Disabled
Input-Default
Input-Error
Table-Default
Dialog-Confirm
```

## 2. React / Vue 组件调用

代码中使用组件属性表达状态，不直接使用 Figma 变体名：

```tsx
<Button type="primary" size="default">查询</Button>
<Button type="text">编辑</Button>
<Input status="error" />
<Table variant="default" />
```

## 3. CSS class 命名

CSS class 使用 BEM 或 kebab-case：

```css
.bms-button
.bms-button--primary
.bms-input--error
.bms-table__header
```

## 4. Token 命名

Token 使用语义命名：

```text
--bms-color-brand
--bms-color-text-primary
--bms-color-bg-page
--bms-color-border-table-line
```

## 禁止事项

- 禁止在代码里使用 `Button-Primary-Hover` 作为 class。
- 禁止混用 `button-primary`、`Button-Primary`、`btnPrimary`。
- 禁止新增没有语义的颜色变量，例如 `--blue1`、`--gray2`。
