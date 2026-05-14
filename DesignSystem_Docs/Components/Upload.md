# Upload

## 1.1 用途

用于文件、页面材料、图片等上传场景。

## 1.2 视觉规范

- 组件：`Upload`
- Style：
  - `Button`：`240px x 62px`
  - `Page`：`320px x 128px`
  - `Picture`：`212px x 106px`
- 颜色：优先使用 Semantic Token，其次 Primitive Token，禁止自定义色值
- 圆角、边框、内边距：待定
- 字体：待定
- 图标：上传图标名称、尺寸、颜色 Token 待定

## 1.3 状态规范

- default：默认上传入口
- hover：待定
- active / focus：待定
- blur：待定
- disabled：待定
- error：待定
- loading：待定
- uploading / success / fail：待定

## 1.4 交互规则

- `Button` 用于紧凑上传入口。
- `Page` 用于文档或附件上传区域。
- `Picture` 用于图片上传区域。
- 上传文件类型、大小限制、进度反馈、失败重试规则待定。

## 1.5 业务场景示例

- 场景 1：【表单业务】中的【附件上传】
- 场景 2：【资料业务】中的【图片上传】

## 1.6 前端适配点

- `style` 映射 `Button | Page | Picture`
- `fileList` 映射文件列表
- `accept` / `maxSize` / `multiple` 规则待定
- 组件名建议：`Upload`

## 1.7 AI 生成约束

- 必须使用系统 `Upload`。
- 禁止自定义上传卡片样式。
- 禁止新增未在 Figma 出现的尺寸、颜色、状态、圆角、阴影。
