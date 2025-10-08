# 此处仅列举我常用的vscode-vim配置
直接加到settings.json中
```json
{
    "vim.easymotion": true,
    "vim.incsearch": true,
    "vim.useSystemClipboard": true,
    "vim.useCtrlKeys": true,
    "vim.hlsearch": true,
    "vim.whichwrap": "h,l,<,>,[,]",
    "vim.insertModeKeyBindings": [
        {
            "before": [
                "j",
                "j"
            ],
            "after": [
                "<Esc>"
            ]
        }
    ],
    "vim.normalModeKeyBindingsNonRecursive": [
        {
            "before": [
                "<leader>",
                "d"
            ],
            "after": [
                "d",
                "d"
            ]
        },
        {
            "before": [
                "<C-n>"
            ],
            "commands": [
                ":nohl"
            ]
        },
        {
            "before": [
                "<C-z>"
            ],
            "commands": [
                "u"
            ]
        },
        {
            "before": [
                "<C-s>"
            ],
            "commands": [
                ":w"
            ]
        },
        {
            "before": [
                "K"
            ],
            "commands": [
                "lineBreakInsert"
            ],
            "silent": true
        },
        {
            "before": [
                " "
            ],
            "after": [
                "leader",
                "leader",
                "leader",
                "b",
                "d",
                "w"
            ]
        }
    ],
    "vim.leader": "<space>",
    "vim.handleKeys": {
        "<C-a>": false,
        "<C-f>": false,
        "<C-c>": false,
        "<C-v>": false,
        "<C-p>": false
    },
    // To improve performance
    "extensions.experimental.affinity": {
        "vscodevim.vim": 1
    },
    "vim.commandLineModeKeyBindings": [],
    "vim.userSystemClipboard": true,
    "editor.wrappingIndent": "none",
}
```