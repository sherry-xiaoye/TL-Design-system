# DetailPage

DetailPage 用于展示对象详情、审批详情、配置详情、只读信息。

## 标准结构

```tsx
<Page>
  <Breadcrumb />
  <PageHeader />
  <DetailHeader />
  <DetailSections />
  <RelatedTable />
</Page>
```

## 模块规则

- PageHeader 展示标题和主要操作。
- DetailHeader 展示核心状态、关键字段。
- DetailSections 使用分组方式展示基础信息、业务信息、操作记录。
- 如果包含明细列表，使用系统 Table。

## 状态规则

- loading：详情数据加载中。
- empty：对象不存在或无可展示内容。
- error：加载失败，提供重试入口。
- permission denied：无权限时展示权限提示。

## 禁止事项

- 禁止把详情页做成大屏展示。
- 禁止大量装饰卡片。
- 禁止字段无分组直接堆叠。
- 禁止硬编码非 Token 色值。
