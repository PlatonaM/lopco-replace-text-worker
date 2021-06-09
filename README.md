## lopco-replace-text-worker

Replace all occurrences of a string inside a file.

### Configuration

`old_text`: Text string to replace.

`new_text`: New text string.

### Inputs

Type: single

`input_file`: File containing text.

### Outputs

Type: single

`output_file`: Result file.

### Description

    {
        "name": "Replace Text",
        "image": "platonam/replace-text-worker:latest",
        "data_cache_path": "/data_cache",
        "description": "Replace all occurrences of a text with another.",
        "configs": {
            "old_text": null,
            "new_text": null
        },
        "input": {
            "type": "single",
            "fields": [
                {
                    "name": "input_file",
                    "media_type": "text/plain",
                    "is_file": true
                }
            ]
        },
        "output": {
            "type": "single",
            "fields": [
                {
                    "name": "output_file",
                    "media_type": "text/plain",
                    "is_file": true
                }
            ]
        }
    }
