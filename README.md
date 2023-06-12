# pipiecd-json-schema
This is the **unofficial** `pipecd.yaml` schema for YAML LSP for the [PipeCD](https://github.com/pipe-cd/pipecd).

*Supported PipeCD Version: v0.43.1*

## How to use

### AstroNvim
```lua
return {
  lsp = {
    config = {
      yamlls = {
        settings = {
          yaml = {
            completion = true,
            schemas = {
              ["https://raw.githubusercontent.com/tetsuya28/pipecd-json-schema/master/pipecd.yaml.json"] = "app.pipecd.yaml",
            },
          },
        },
      },
    },
  },
}
```

### Coc
[neoclide/coc.nvim: Nodejs extension host for vim & neovim, load extensions like VSCode and host language servers.](https://github.com/neoclide/coc.nvim)

In Coc, hook open config with `:CocConfig` in vim, and append the following lines.

```json
{
  ...,
  "yaml.schemas": {
    "https://raw.githubusercontent.com/tetsuya28/pipecd-json-schema/master/pipecd.yaml.json": ["*pipecd.yaml", "*pipe.yaml"]
  }
}
```

### VSCode
In VSCode setting.json, you can add these following lines.

```json
    "yaml.format.enable": true,
    "yaml.completion": true,
    "yaml.validate": true,
    "yaml.hover": true,
    "yaml.schemas": {
        "https://raw.githubusercontent.com/tetsuya28/pipecd-json-schema/master/pipecd.yaml.json": ["*pipecd.yaml", "*pipe.yaml"],
    },
```

## Contribute
Welcome to update schema!!
