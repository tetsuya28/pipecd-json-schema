# pipiecd-json-schema
This is the **unofficial** `pipecd.yaml` schenma for YAML LSP for the [PipeCD](https://github.com/pipe-cd/pipecd).

## How to use
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
