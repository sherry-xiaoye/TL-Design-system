# Grid

The design system is optimized for desktop BMS screens.

## Desktop Shell

| Region | Size |
|---|---:|
| Canvas | 1440 x 900 reference |
| Header | 56px height |
| Sidebar | 180px width |
| Body x offset | 180px |
| Body y offset | 56px |
| Body size | 1260 x 844 |
| Body padding | 20px |
| Main content width | 1220px |

## Content Grid

- Use `1220px` as the default inner content width in the desktop body.
- Filter bars and table toolbars usually span `1220px`.
- Multi-column form examples use 360px field columns inside a 1180px container.
- Card grids in dashboard/list pages divide 1220px into three columns with 20px gutters.

## Rules

- Header and sidebar are fixed shell regions.
- Body scrolls independently when content is taller than the viewport.
- Place main content at `x=20`, `y=20` inside body unless a pattern states otherwise.
- Use full-width table/card containers rather than floating decorative cards.
- Keep dense operational screens scannable: align labels, inputs, table columns, and toolbar actions to a clear grid.

