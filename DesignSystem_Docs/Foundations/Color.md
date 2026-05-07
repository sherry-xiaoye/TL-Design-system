# Color

本文件基于已提供的 Figma Token JSON 整理。颜色必须使用语义 Token，不得随意硬编码。

## 已确认颜色 Token

| CSS Variable | Value | Figma Token Source |
|---|---|---|
| `--bms-color-brand` | `#3D71FF` | `Text-brand` |
| `--bms-color-text-primary` | `#303133` | `Text-primary` |
| `--bms-color-text-table-header` | `#666666` | `Text-TableHeader` |
| `--bms-color-text-secondary-disabled` | `#A0A1A2` | `Text-Secondary-Disable Font` |
| `--bms-color-text-tips` | `#C0C1C6` | `Text-Tips` |
| `--bms-color-border-table-line` | `#E1E2E5` | `Table-Line&Dis-Line` |
| `--bms-color-border-divider` | `#EDEDEF` | `Divider-Border` |
| `--bms-color-bg-menu` | `#F2F2F3` | `Background-Menu` |
| `--bms-color-bg-table-header` | `#F2F2F3` | `Background-TableHeader` |
| `--bms-color-bg-page` | `#F7F8F9` | `Background-Page` |
| `--bms-color-bg-white` | `#FFFFFF` | `White` |
| `--bms-color-status-warning` | `#F69825` | `Text-Warning` |
| `--bms-color-status-success` | `#1EA285` | `Text-Finish` |
| `--bms-color-status-error` | `#F96C6C` | `Text-Error` |
| `--bms-color-icon-primary-select` | `#666666` | `Icon-primary-Select` |
| `--bms-color-icon-secondary-disabled` | `#A0A1A2` | `Icon-secondary-Disable` |
| `--bms-color-icon-thirdly-normal` | `#C0C1C6` | `Icon-Thirdly-Normol` |
| `--bms-color-bg-info-weak` | `#F1F7FF` | `Backgroundcolor- Normal` |
| `--bms-color-bg-success-weak` | `#E8FAF4` | `Backgroundcolor- Success` |
| `--bms-color-bg-warning-weak` | `#FFF5E3` | `Backgroundcolor- Warning` |
| `--bms-color-bg-error-weak` | `#FFEEEE` | `Backgroundcolor- Error` |
| `--bms-color-bg-brand` | `#3D71FF` | `Backgroundcolor- Brnd` |

## 使用规则

- 页面背景：`--bms-color-bg-page`。
- 内容容器和弹窗背景：`--bms-color-bg-white`。
- 主操作、选中态、品牌强调：`--bms-color-brand`。
- 表格表头背景：`--bms-color-bg-table-header`。
- 表格分割线：`--bms-color-border-table-line`。
- 输入框边框优先使用：`--bms-color-border-table-line`。
- 分割线、弱边框：`--bms-color-border-divider`。

## 禁止事项

- 禁止使用未登记颜色。
- 禁止使用 `#1677ff`、`red`、`blue`、`rgba(...)` 替代系统 Token。
- 禁止为单个页面临时创建品牌色、表头色、边框色。
