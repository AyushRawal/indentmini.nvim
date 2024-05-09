# indentmini.nvim
A minimal less than ~130 lines and blazing fast indentline plugin. no much more features but useful!

![old](https://github.com/nvimdev/indentmini.nvim/assets/41671631/d836db79-4c41-45bc-99cb-d9f807dfe9af)

## Install

install with any plugin management or default vim package.

## Config

available config values in setup table.

- char     -- string type default is `│`,
- current  -- boolean highlight current indent level
- exclude  -- table  type add exclude filetype in this table ie `{ 'markdown', 'xxx'}`

```lua
config = function()
    require("indentmini").setup() -- use default config
end,
```

## Highlight

if your colorscheme not config the `IndentLine*` relate highlight group you should config it in
your neovim config.

```lua
-- Colors are applied automatically based on user-defined highlight groups.
-- There is no default value.
vim.cmd.highlight('IndentLine guifg=#123456')
-- Current indent line highlight
vim.cmd.highlight('IndentLineCurrent guifg=#123456')
```

## Tips

set the `updatetime` to 100 will have a better experience when edit in insert
mode.

## License MIT
