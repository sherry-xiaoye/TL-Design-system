# FormPage

FormPage 用于新增、编辑、配置、审批等表单录入场景。

## 标准结构

```tsx
<Page>
  <Breadcrumb />
  <PageHeader />
  <FormArea />
  <FooterActions />
</Page>
```

## 模块顺序

1. Breadcrumb
2. PageHeader
3. FormArea
4. FooterActions

不得随意调整模块顺序。

## FormArea 规则

- 表单项应按业务分组。
- 每组可使用 Block Header 或 Card，是否使用 Card 视复杂度而定。
- Label 对齐方式：待定。
- 表单项间距：待定；如果项目已有 spacing 变量，复用项目变量。
- 必填项必须有明确标识。
- 错误提示必须展示在对应输入项下方。
- 表单组件必须使用系统 Input / Select / Radio / Checkbox / DatePicker / Switch / Upload。

## FooterActions 规则

- 底部操作按钮包含主操作和次操作。
- 主操作一般为“保存”“提交”“确定”。
- 次操作一般为“取消”“返回”。
- 异步提交时主按钮必须进入 loading。
- 高危提交必须二次确认。

## 校验规则

- 必填字段不能为空。
- 格式校验必须给出明确错误文案。
- 服务端错误必须映射到对应字段或展示全局错误提示。
- 提交失败必须保留用户已填写内容。

## 状态规则

| 状态 | 规则 |
|---|---|
| loading | 初始化数据或提交时展示 loading |
| disabled | 不可编辑字段使用禁用或只读态，具体待定 |
| error | 字段下方显示错误提示 |
| permission denied | 无权限时禁止展示可编辑表单 |
| submit success | 给出成功反馈并按业务跳转或留在当前页 |

## 禁止事项

- 禁止自由布局导致 Label 和字段不对齐。
- 禁止用普通 Input 手写日期、时间、选择器。
- 禁止提交时无 loading。
- 禁止校验失败只改变颜色但无错误文案。
- 禁止把表单页做成营销落地页。
- 禁止多层卡片嵌套。

## AI 生成约束

- 生成 FormPage 时必须读取相关表单组件文档。
- 所有颜色必须来自 Token。
- 未确认尺寸标记为待定，不得伪造 Token。
- 输出代码后必须按 `Guidelines/AI_Output_Checklist.md` 自检。
