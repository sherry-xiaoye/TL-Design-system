# Grid

## 当前状态

当前上传的 JSON 中未提供 Grid / Breakpoint Token。栅格列数、断点、页面最大宽度均为待定。

## 建议规则（非 Token）

- 后台页面可采用 8px 基础节奏，但该规则当前为待确认。
- 筛选表单建议每行最多 4 项，但具体列宽待定。
- 复杂业务布局可以使用 CSS Grid / Flex，但必须保持对齐和信息可读。

## 禁止事项

- 禁止伪造 Grid Token。
- 禁止在不同页面随意切换布局节奏。
- 禁止为了视觉装饰牺牲表格和表单效率。

## Desktop Shell

| 区域 | 规格 |
|---|---|
| Header | 高度 `56px` |
| Sidebar-Left| 宽度 `180px` |
| Body | `x=180`, `y=56` |
| Body Padding | `20px` |

## 规则

- Header / Sidebar-Left / Body 是 BMS 标准壳结构。
- 表格、筛选区、工具栏默认对齐到主内容宽度。
- 响应式断点：`待定`。
- Body区域 8珊格‘待定’
- 禁止随意切换页面栅格节奏。
