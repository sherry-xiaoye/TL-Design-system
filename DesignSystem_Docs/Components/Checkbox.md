# Checkbox

## 1.1 用途

用于多选、批量选择、表格行选择和部分选中场景。

## 1.2 视觉规范

- 组件：`Checkbox`
- 颜色：优先使用 Semantic Token，其次 Primitive Token，禁止自定义色值
- 尺寸：待定
- 字体：待定
- 图标：勾选、半选图标样式待定

## 1.3 状态规范

- default：`Normol`
- selected：`Select`
- disabled：`Disable`
- selected disabled：`SelectDisable`
- indeterminate：`Selectpart`
- hover：待定
- active / focus：待定
- blur：待定
- error：待定
- loading：不适用

## 1.4 交互规则

- 支持多项选择。
- 表格全选场景需支持半选状态。
- 禁用状态不可点击。
- 点击文字或勾选框均可切换状态，具体点击热区待定。

## 1.5 业务场景示例

- 场景 1：【表格业务】中的【行选择 / 批量操作】
- 场景 2：【筛选业务】中的【多条件选择】

## 1.6 前端适配点

- `checked` 映射选中状态
- `indeterminate` 映射 `Selectpart`
- `disabled` 映射禁用状态
- 组件名建议：`Checkbox` / `CheckboxGroup`

## 1.7 AI 生成约束

- 必须使用系统 `Checkbox`。
- 禁止用图标或 div 模拟复选框。
- 必须保留半选状态。
- 禁止新增未在 Figma 出现的状态、尺寸、颜色、圆角、阴影。
