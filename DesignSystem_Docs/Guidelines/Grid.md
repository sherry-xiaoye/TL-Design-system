# Grid

## 基础规则

- 当前颜色 Token 已确认，尺寸 Token 未从 JSON 中确认。
- 间距、断点、栅格列数如未在项目变量中存在，应标记为“待定”。
- 不得把未确认尺寸写成 Token。

## 推荐写法

```css
/* 可复用项目既有变量；如项目尚未定义，则标记为待定 */
gap: var(--project-space-16); /* 如存在 */
gap: /* 待定 */;
```

## 禁止事项

- 禁止随意使用 5px、7px、13px、19px 等非系统间距。
- 禁止为了让页面“好看”临时写一套 spacing Token。
- 禁止伪造未确认的 grid / radius / shadow Token。
