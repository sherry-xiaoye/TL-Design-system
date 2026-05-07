# Guidelines

## 设计原则

BMS 是高密度后台管理系统，核心任务是查询、录入、配置、审批和监控。

### 1. 信息优先

- 页面结构服务于业务信息，不以视觉装饰为主。
- 表格、表单、筛选、详情和弹窗是核心界面模式。
- 重要信息优先展示，次要信息弱化处理。

### 2. 操作清晰

- 每个页面只保留必要主操作。
- 主操作使用 Primary Button。
- 次要操作使用 Default Button。
- 表格行内操作优先使用 Text Button。
- 删除、停用、作废等高危操作必须二次确认。

### 3. 视觉克制

- 页面背景使用 `--bms-color-bg-page`。
- 内容容器使用 `--bms-color-bg-white`。
- 表格表头使用 `--bms-color-bg-table-header`。
- 禁止大面积渐变、装饰插画、光斑、强阴影。

### 4. 组件一致

- 优先使用系统组件。
- 禁止重复创建 Button、Input、Select、Table、Dialog 等基础组件。
- 禁止用 div / span 模拟基础组件。

### 5. 状态完整

列表、表格、详情、图表、表单提交必须考虑：

- loading
- empty
- error
- disabled
- permission denied（如业务存在权限）
