#### Description

    {
        "name": "Replace Text",
        "image": "platonam/replace-text-worker:dev",
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
