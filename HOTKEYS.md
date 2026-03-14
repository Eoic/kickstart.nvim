# Neovim Hotkey Reference

> Leader key: **Space**

## Essential Editor

| Key | Mode | Action |
|-----|------|--------|
| `<Esc>` | Normal | Clear search highlights |
| `<C-s>` | Normal/Insert | Save file |
| `<leader>q` | Normal | Open diagnostic quickfix list |
| `<Esc><Esc>` | Terminal | Exit terminal mode |

## Window Navigation

| Key | Mode | Action |
|-----|------|--------|
| `<C-h>` | Normal | Focus left window |
| `<C-l>` | Normal | Focus right window |
| `<C-j>` | Normal | Focus lower window |
| `<C-k>` | Normal | Focus upper window |

## Search (Telescope) — `<leader>s`

| Key | Action |
|-----|--------|
| `<leader>sf` | Search files |
| `<leader>sg` | Search by grep (live grep) |
| `<leader>sw` | Search current word |
| `<leader>sh` | Search help tags |
| `<leader>sk` | Search keymaps |
| `<leader>ss` | Search select (Telescope pickers) |
| `<leader>sd` | Search diagnostics |
| `<leader>sr` | Resume last search |
| `<leader>s.` | Search recent files |
| `<leader>s/` | Search in open files |
| `<leader>sn` | Search Neovim config files |
| `<leader><leader>` | Find open buffers |
| `<leader>/` | Fuzzy search in current buffer |

## LSP — Code Navigation

| Key | Action |
|-----|--------|
| `gd` | Go to definition |
| `gr` | Go to references |
| `gI` | Go to implementation |
| `gD` | Go to declaration |
| `<leader>D` | Go to type definition |
| `<leader>ds` | Document symbols |
| `<leader>ws` | Workspace symbols |

## LSP — Refactoring

| Key | Mode | Action |
|-----|------|--------|
| `<leader>rn` | Normal | Rename symbol |
| `<leader>ca` | Normal/Visual | Code action |
| `<leader>f` | Normal/Visual | Format buffer |
| `<leader>th` | Normal | Toggle inlay hints |

## Completion (Insert Mode)

| Key | Action |
|-----|--------|
| `<C-n>` | Next completion item |
| `<C-p>` | Previous completion item |
| `<C-y>` | Confirm completion |
| `<C-Space>` | Trigger completion manually |
| `<C-b>` | Scroll docs back |
| `<C-f>` | Scroll docs forward |
| `<C-l>` | Jump to next snippet placeholder |
| `<C-h>` | Jump to previous snippet placeholder |

## Git (Gitsigns) — `<leader>h`

| Key | Mode | Action |
|-----|------|--------|
| `]c` | Normal | Next git change |
| `[c` | Normal | Previous git change |
| `<leader>hs` | Normal/Visual | Stage hunk |
| `<leader>hr` | Normal/Visual | Reset hunk |
| `<leader>hS` | Normal | Stage entire buffer |
| `<leader>hu` | Normal | Undo stage hunk |
| `<leader>hR` | Normal | Reset entire buffer |
| `<leader>hp` | Normal | Preview hunk inline |
| `<leader>hb` | Normal | Blame current line |
| `<leader>hd` | Normal | Diff against index |
| `<leader>hD` | Normal | Diff against last commit |
| `<leader>tb` | Normal | Toggle line blame |
| `<leader>tD` | Normal | Toggle show deleted lines |

## Debugging (DAP)

| Key | Action |
|-----|--------|
| `<F5>` | Start / Continue |
| `<F1>` | Step into |
| `<F2>` | Step over |
| `<F3>` | Step out |
| `<F7>` | Toggle debug UI |
| `<leader>b` | Toggle breakpoint |
| `<leader>B` | Set conditional breakpoint |

## File Explorer (Neo-tree)

| Key | Action |
|-----|--------|
| `\` | Toggle Neo-tree file explorer |

## Mini.nvim Plugins

- **mini.ai** — Enhanced text objects (`a`/`i` motions around brackets, quotes, function args, etc.)
- **mini.surround** — Add/delete/change surroundings (brackets, quotes, tags):
  - `sa` + motion + char — Add surrounding
  - `sd` + char — Delete surrounding
  - `sr` + old + new — Replace surrounding

## Built-in Vim Motions Worth Practicing

| Key | Action |
|-----|--------|
| `ciw` / `diw` | Change/delete inner word |
| `ci"` / `di"` | Change/delete inside quotes |
| `%` | Jump to matching bracket |
| `*` / `#` | Search word under cursor forward/backward |
| `gg` / `G` | Top/bottom of file |
| `{` / `}` | Jump by paragraph |
| `zz` / `zt` / `zb` | Center/top/bottom cursor on screen |
| `<C-o>` / `<C-i>` | Jump back/forward in jumplist |
| `<C-d>` / `<C-u>` | Half-page down/up |
| `.` | Repeat last change |
| `q{a-z}` / `@{a-z}` | Record/play macro |

## Practice Suggestions

1. **Start with search** — `<leader>sf`, `<leader>sg`, and `<leader>/` will transform how you navigate
2. **Use LSP navigation** — `gd` and `gr` replace manual searching for definitions
3. **Learn git hunks** — `]c`/`[c` to jump between changes, `<leader>hp` to preview
4. **Master completion** — `<C-n>`/`<C-p>`/`<C-y>` flow in insert mode
5. **Use mini.surround** — `sa`/`sd`/`sr` for quick bracket/quote manipulation
6. **Try which-key** — Press `<leader>` and wait to see all available options
