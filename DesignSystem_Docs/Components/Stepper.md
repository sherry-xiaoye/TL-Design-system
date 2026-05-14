# Stepper

## 1.1 用途

用于数值递增、递减输入，适合有明确范围或步长的数值字段。

## 1.2 视觉规范

- 组件：`Stepper`
- 尺寸：`132px x 36px`
- 颜色：优先使用 Semantic Token，其次 Primitive Token，禁止自定义色值
- 内边距：待定
- 圆角：待定
- 边框：待定
- 字体：待定
- 图标：增减图标名称、尺寸、颜色 Token 待定

## 1.3 状态规范

- default：`Default`
- hover：`Hover`
- active / focus：`Active`
- blur：`Blur`
- disabled：`Disabled`
- error：待定
- loading：不适用

## 1.4 交互规则

- 点击加号增加数值。
- 点击减号减少数值。
- 可输入范围、步长、最小值、最大值规则待定。
- 禁用状态不可输入、不可点击。

## 1.5 业务场景示例

- 场景 1：【配置业务】中的【数量设置】
- 场景 2：【表单业务】中的【排序值填写】

## 1.6 前端适配点

- `value` 映射当前数值
- `min` / `max` / `step` 映射范围与步长，具体规则待定
- `disabled` 映射禁用状态
- Figma 状态名统一为 `Blur`，代码中映射为 `blur`

## 1.7 AI 生成约束

- 必须使用系统 `Stepper`。
- 禁止用 Input + Button 自行拼装。
- 禁止新增未在 Figma 出现的状态名。
- 禁止新增未在 Figma 出现的状态、尺寸、颜色、圆角、阴影。
