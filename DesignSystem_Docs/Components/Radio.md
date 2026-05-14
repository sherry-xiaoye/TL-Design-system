# Radio

## 1.1 用途

用于少量互斥选项选择。适合选项数量较少、需要直接展示全部选项的业务场景。

## 1.2 视觉规范

- 组件：`Radio`
- 颜色：优先使用 Semantic Token，其次 Primitive Token，禁止自定义色值
- 尺寸：待定
- 字体：待定
- 图标：单选圆点样式待定

## 1.3 状态规范

- default：`Default`
- hover：待定
- active / focus：待定
- blur：待定
- disabled：`Disabled`
- selected：`Selected`
- selected disabled：`SelectedDisabled`
- error：待定
- loading：不适用

## 1.4 交互规则

- 同一组内只能选择一个选项。
- 点击选项或文字区域后切换选中项。
- 禁用状态不可点击。

## 1.5 业务场景示例

- 场景 1：【筛选业务】中的【状态单选】
- 场景 2：【表单业务】中的【类型选择】

## 1.6 前端适配点

- `value` 映射当前选中值
- `options` 映射选项列表
- `disabled` 映射禁用状态
- 组件名建议：`Radio` / `RadioGroup`

## 1.7 AI 生成约束

- 必须使用系统 `Radio`。
- 禁止用按钮或标签模拟单选。
- 禁止新增未在 Figma 出现的状态、尺寸、颜色、圆角、阴影。
