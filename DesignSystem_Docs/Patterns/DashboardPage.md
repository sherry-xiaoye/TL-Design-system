# DashboardPage

DashboardPage 用于概览关键指标和管理状态，不等同于数据大屏。

## 标准结构

```tsx
<Page>
  <Breadcrumb />
  <PageHeader />
  <MetricCards />
  <ChartArea />
  <DataTable />
</Page>
```

## 规则

- Dashboard 保持后台系统风格，不使用大屏、炫酷、渐变、光效。
- 指标卡片使用系统 Card。
- 图表颜色优先使用 Token，未定义图表色时标记为待定。
- 图表必须考虑 loading / empty / error。
- 可下钻的数据必须提供明确入口。

## 禁止事项

- 禁止大屏风。
- 禁止深色炫酷背景，除非产品另有独立主题。
- 禁止装饰性图表。
- 禁止无数据状态下显示假图表。
