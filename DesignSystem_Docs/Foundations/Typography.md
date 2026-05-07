# Typography

## 当前状态

当前上传的 JSON 中未提供完整 Typography Token。因此字体族、字号、字重、行高均标记为待定，不能伪造成 Token。

## 建议规则（非 Token）

以下为后台系统常见建议，用于设计确认前的占位，不得写入 `tokens.css` 作为已确认 Token：

| 项目 | 建议 | 状态 |
|---|---|---|
| 字体族 | PingFang SC / Arial / sans-serif | 待定 |
| 正文字号 | 14px | 待定 |
| 辅助字号 | 12px | 待定 |
| 页面标题 | 16px / 18px | 待定 |
| 字重 | regular / medium | 待定 |
| 行高 | 待定 | 待定 |

## 文本颜色

文本颜色使用已确认颜色 Token：

- 主文本：`--bms-color-text-primary`
- 表头文本：`--bms-color-text-table-header`
- 禁用文本：`--bms-color-text-secondary-disabled`
- 提示文本：`--bms-color-text-tips`

## 禁止事项

- 禁止把建议字号写入 Token。
- 禁止为单个页面单独定义标题体系。
- 禁止使用过大的营销标题字号。
