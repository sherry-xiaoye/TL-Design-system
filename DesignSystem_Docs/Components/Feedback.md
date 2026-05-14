# Feedback

## 使用场景

Feedback 是反馈组件族，用于在 BMS 系统中向用户说明操作结果、系统状态、异常原因、加载进度或无数据状态。

Feedback 不作为单一组件直接使用，应根据反馈发生的位置、持续时间、是否阻断操作、是否需要用户处理来选择具体组件。

| 反馈场景 | 使用组件 | 使用条件 | 是否自动消失 | 是否阻断操作 |
| --- | --- | --- | --- | --- |
| 页面内持续提示 | Alert | 当前页面或当前模块需要持续展示说明、警告、成功、失败信息 | 否 | 否 |
| 全局异步通知 | Notification | 后台任务、异步操作、跨页面结果通知 | 待定 | 否 |
| 轻量即时反馈 | Toast | 保存、复制、删除等操作后的短反馈 | 是 | 否 |
| 数据加载等待 | Loading | 页面、区块、表格、按钮处于请求中或处理中 | 请求结束后消失 | 视遮罩范围而定 |
| 可量化任务进度 | Progress | 上传、导入、批处理等可展示进度百分比的任务 | 任务结束后消失或保留结果，规则待定 | 否 |
| 空状态 / 异常占位 | Default-Image | 空数据、404、无权限、错误页等占位反馈 | 否 | 视页面类型而定 |
| 流程结果反馈 | Result | 表单创建、提交、审批等流程结束后，需要展示成功或失败结果并引导下一步 | 否 | 是 |

使用判断：

- 用户完成一个轻量操作后，只需要短提示，使用 `Toast`。
- 当前页面需要持续展示一段提示或风险说明，使用 `Alert`。
- 操作结果来自异步任务，且用户可能已经离开当前上下文，使用 `Notification`。
- 用户正在等待数据或处理结果，使用 `Loading`。
- 任务可以量化进度，使用 `Progress`。
- 列表、搜索、页面内容为空或不可访问，使用 `Default-Image`。
- 流程已经结束并需要承接下一步动作，使用 `Result`。

## 允许变体

Feedback 组件族已确认包含以下组件与变体：

| 组件 | Figma 已确认变体 | 说明 |
| --- | --- | --- |
| Alert | `Style=Info / Success / Warning / Error`，`State=Icon / Link / Btn` | 页面内提示，可带关闭图标、链接或按钮 |
| Notification | `Type=Info / Success / Warning / Error` | 全局通知提醒 |
| Progress | `Type` / `Action`，具体枚举待定 | 进度反馈 |
| Loading | `Style`，具体枚举待定 | 加载等待 |
| Toast | `State` / `Closable`，具体枚举待定 | 轻提示 |
| Default-Image | `State=Empty / 404 / AccessDenied / Error` | 缺省图与异常占位 |
| Result | `State=Success / Error` | 结果反馈 |

状态类型使用语义：

| 类型 | 使用语义 |
| --- | --- |
| Info | 中性说明、常规提示 |
| Success | 成功、完成、正向结果 |
| Warning | 风险、预警、需注意但未失败 |
| Error | 失败、异常、阻断问题 |

## 尺寸与视觉

Feedback 组件族不统一描述视觉样式。各组件的尺寸、颜色、间距、圆角、阴影、图标、字体必须分别以对应 Figma 组件和 Token 为准。

通用规则：

- 颜色：优先使用 Semantic Token，其次 Primitive Token，禁止自定义色值。
- 尺寸：只记录 Figma 或 Token 已确认的宽 / 高、内边距、圆角、边框。
- 字体：只使用 Figma 或 Token 已确认的字号、字重、颜色、对齐方式。
- 图标：只使用 Figma 已出现的图标名称、尺寸和颜色 Token。
- 未被 Figma 或 Token 确认的视觉值统一标记为 `待定`。
- 不允许把 Alert、Notification、Toast、Result、Loading、Progress、Default-Image 的样式合并成一套规则。

已确认的 Result 视觉信息：

- Result 支持 `Success` 与 `Error`。
- 结果图标尺寸使用 `Size/48*48`。
- 成功图标使用 `Icon/Success`。
- 失败图标使用 `Icon/Danger`。
- 主文案使用 `Text/Primary` 和 `Body/次文本`。
- 按钮组复用 Button 组件样式。
- Error 结果中的错误原因区域背景使用 `Background/Zebra`。
- Error 结果中的解决办法使用文本按钮样式，文字颜色使用 `Text/brand`。

其他反馈组件视觉规范见对应组件文档：

- `Alert.md`
- `Notification.md`
- `Toast.md`
- `Loading.md`
- `Progress.md`
- `Default.md`

## 状态

Feedback 组件族的状态必须按组件分别定义，不做统一状态套用。

| 组件 | 已确认状态 / 类型 | 状态说明 |
| --- | --- | --- |
| Alert | `Info / Success / Warning / Error`，`Icon / Link / Btn` | 页面内提示状态，支持不同右侧操作形式 |
| Notification | `Info / Success / Warning / Error` | 全局通知类型 |
| Toast | `Info / Success / Warning / Error`，`Closable` 规则待定 | 短反馈状态 |
| Loading | `loading` | 加载中 |
| Progress | `processing / success / error`，具体以组件文档为准 | 进度状态 |
| Default-Image | `Empty / 404 / AccessDenied / Error` | 缺省与异常状态 |
| Result | `Success / Error` | 流程结果状态 |

Result 状态规范：

- `Success`：用于流程完成、创建成功、提交成功等正向结果；展示成功图标、结果文案和后续操作按钮。
- `Error`：用于流程提交失败、创建失败等阻断结果；展示失败图标、失败文案、错误原因、解决办法入口和后续操作按钮。
- `Warning`：Figma 当前 Result 节点未提供，标记为 `待定`。
- `Info`：Figma 当前 Result 节点未提供，标记为 `待定`。
- `Loading`：Result 不承载加载态；流程处理中应使用 `Loading` 或按钮 loading，规则待定。
- `Disabled`：Result 不定义整体禁用态；按钮禁用需继承 Button 组件规范。

## 交互规则

反馈选择规则：

- `Toast` 用于轻量操作后的即时反馈，不承载长文本、复杂操作或持续说明。
- `Alert` 用于当前页面内需要持续阅读的信息，不自动消失，是否可关闭由业务配置决定。
- `Notification` 用于异步结果或系统级通知，不应打断当前页面操作。
- `Loading` 用于请求中、提交中、处理中，必须在请求结束后移除。
- `Progress` 用于可量化进度，不应用普通 Loading 替代可明确展示百分比的任务。
- `Default-Image` 用于内容缺省、无权限、404、系统错误等页面或区块占位。
- `Result` 用于流程终点，必须给出明确结果和下一步操作。

Result 交互规则：

- Success 结果必须提供至少一个后续操作，例如查看结果、继续创建、返回列表，具体动作以业务为准。
- Error 结果必须展示失败原因或解决入口；如果原因来自接口，字段映射规则为 `待定`。
- Error 结果应提供返回修改、回到列表或重试等操作，具体按钮数量和优先级以业务为准。
- Result 页面不自动关闭。
- Result 中按钮行为由业务路由或操作回调决定，跳转规则为 `待定`。

异常场景处理：

- 请求中使用 `Loading`，请求成功后根据结果进入正常内容、`Toast`、`Alert` 或 `Result`。
- 请求失败且影响当前页面继续操作时，优先使用 `Alert`、`Result` 或 `Default-Image`，不只使用 `Toast`。
- 空列表、无搜索结果、无权限不可用 `Toast` 替代，应使用 `Default-Image` 或对应页面空状态。

## 前端适配

组件选择映射：

| 前端场景 | 推荐组件 | 关键字段 |
| --- | --- | --- |
| 操作成功短提示 | `Toast` | `type`, `message`, `duration` |
| 页面内提示 | `Alert` | `type`, `message`, `closable`, `action` |
| 异步通知 | `Notification` | `type`, `title`, `message`, `duration` |
| 请求等待 | `Loading` | `loading`, `text`, `fullscreen`, `target` |
| 进度展示 | `Progress` | `percent`, `status`, `type` |
| 空状态 | `Default-Image` | `state`, `description`, `action` |
| 结果页 | `Result` | `state`, `title`, `reasons`, `actions` |

Result Props / Variant 映射：

```tsx
<Result
  state="Success"
  title="#表单名称#创建成功"
  actions={[
    { type: "secondary", text: "查看表单" },
    { type: "primary", text: "继续创建" }
  ]}
/>

<Result
  state="Error"
  title="#表单名称#提交失败"
  reasons={[
    { text: "#错误原因1#", actionText: "解决办法" },
    { text: "#错误原因2#", actionText: "解决办法" }
  ]}
  actions={[
    { type: "secondary", text: "回到列表" },
    { type: "primary", text: "返回修改" }
  ]}
/>
```

数据回显规则：

- Result 的标题、错误原因、解决办法、按钮文案均由业务数据或配置传入。
- 错误原因字段、解决办法链接字段、按钮跳转字段的接口字段映射规则：`待定`。
- Toast / Notification / Alert 的消息内容字段映射规则：`待定`。

样式类名 / 组件名规范：

- 组件名使用 `Alert`、`Notification`、`Toast`、`Loading`、`Progress`、`DefaultImage`、`Result`。
- 样式类名规范：`待定`。
- 不允许在业务页面临时创建反馈类组件替代系统组件。

## 禁止事项

- 禁止把 Feedback 当成一个可直接调用的单一组件。
- 禁止把不同反馈组件的视觉样式统一描述或互相套用。
- 禁止用 Toast 承载需要持续阅读、需要处理或阻断流程的反馈。
- 禁止用 Alert 替代结果页。
- 禁止用 Notification 替代页面内必须保留的错误说明。
- 禁止用 Loading 替代可量化的 Progress。
- 禁止用 Toast 替代空状态、404、无权限或系统错误页。
- 禁止自定义反馈颜色、图标、圆角、阴影和状态。
- 禁止新增未在 Figma 出现的反馈状态和尺寸。

## AI 生成约束

- 生成反馈内容前，必须先判断反馈场景，再选择具体反馈组件。
- 必须优先使用系统定义的 Feedback 子组件和组件变体。
- 必须使用系统定义的 Token 和 Figma 已确认的组件变体。
- 禁止把 `Info / Success / Warning / Error` 简单套用于所有反馈组件；只有 Figma 或组件文档确认的状态才可使用。
- 异步页面必须考虑 `loading / success / error / empty`，但展示组件需按场景选择。
- 列表和搜索结果必须考虑 empty 状态。
- 提交流程必须考虑 success / error 结果；需要流程终点展示时使用 `Result`。
- 失败反馈必须提供可理解的原因或下一步处理方式；无法确认时标记为 `待定`。
- 禁止新增未在 Figma 出现的尺寸、颜色、状态、圆角、阴影。
- 未经 Figma 或 Token 确认的值必须标记为 `待定`。
