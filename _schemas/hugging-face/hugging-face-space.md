---
description: Schema for a Space (interactive ML application) hosted on the Hugging Face Hub, including runtime configuration, SDK, hardware, and repository metadata.
layout: schema
name: Hugging Face Space
properties_list:
- description: Internal unique identifier for the Space
  name: _id
  type: string
- description: Space repository ID in the format author/space-name
  name: id
  type: string
- description: Author or organization that owns the Space
  name: author
  type: string
- description: Latest Git commit SHA
  name: sha
  type: string
- description: Timestamp of the last modification
  name: lastModified
  type: string
- description: Timestamp when the Space was created
  name: createdAt
  type: string
- description: Whether the Space is private
  name: private
  type: boolean
- description: Whether the Space has been disabled
  name: disabled
  type: boolean
- description: Tags associated with the Space
  name: tags
  type: array
- description: Number of likes/favorites
  name: likes
  type: integer
- description: SDK framework used to build the Space
  name: sdk
  type: string
- description: Version of the SDK
  name: sdk_version
  type: string
- description: Python version used
  name: python_version
  type: string
- description: Main application file (e.g., app.py)
  name: app_file
  type: string
- description: Port the application listens on (for Docker Spaces)
  name: app_port
  type: integer
- description: Emoji displayed next to the Space name
  name: emoji
  type: string
- description: Gradient start color for the Space card
  name: colorFrom
  type: string
- description: Gradient end color for the Space card
  name: colorTo
  type: string
- description: Whether the Space is pinned on the author's profile
  name: pinned
  type: boolean
- description: License identifier
  name: license
  type: string
- description: Brief description shown on the Space card
  name: short_description
  type: string
- description: Model IDs used by this Space
  name: models
  type: array
- description: Dataset IDs used by this Space
  name: datasets
  type: array
- description: Runtime status and configuration
  name: runtime
  type: object
- description: Files in the Space repository
  name: siblings
  type: array
- description: Parsed metadata from the Space card YAML front matter
  name: cardData
  type: object
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-space-schema.json
slug: hugging-face-space
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://huggingface.co/schemas/space.json\",\n  \"title\": \"Hugging Face Space\",\n  \"description\": \"Schema for a Space (interactive ML application) hosted on the Hugging Face Hub, including runtime configuration, SDK, hardware, and repository metadata.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\"\n  ],\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Internal unique identifier for the Space\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Space repository ID in the format author/space-name\",\n      \"examples\": [\n        \"stabilityai/stable-diffusion\",\n        \"huggingface/chat-ui\",\n        \"gradio/hello-world\"\n      ]\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"Author or organization that owns the Space\"\n    },\n    \"sha\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Latest Git commit SHA\",\n      \"pattern\": \"^[0-9a-f]{40}$\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last modification\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the Space was created\"\n    },\n    \"private\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Space is private\",\n      \"default\": false\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Space has been disabled\",\n      \"default\": false\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags associated with the Space\"\n    },\n    \"likes\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of likes/favorites\",\n      \"minimum\"\
  : 0\n    },\n    \"sdk\": {\n      \"type\": \"string\",\n      \"description\": \"SDK framework used to build the Space\",\n      \"enum\": [\n        \"gradio\",\n        \"streamlit\",\n        \"docker\",\n        \"static\"\n      ]\n    },\n    \"sdk_version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the SDK\"\n    },\n    \"python_version\": {\n      \"type\": \"string\",\n      \"description\": \"Python version used\"\n    },\n    \"app_file\": {\n      \"type\": \"string\",\n      \"description\": \"Main application file (e.g., app.py)\",\n      \"default\": \"app.py\"\n    },\n    \"app_port\": {\n      \"type\": \"integer\",\n      \"description\": \"Port the application listens on (for Docker Spaces)\"\n    },\n    \"emoji\": {\n      \"type\": \"string\",\n      \"description\": \"Emoji displayed next to the Space name\"\n    },\n    \"colorFrom\": {\n      \"type\": \"string\",\n      \"description\": \"Gradient start color for the Space card\"\
  ,\n      \"pattern\": \"^#[0-9a-fA-F]{6}$|^[a-z]+$\"\n    },\n    \"colorTo\": {\n      \"type\": \"string\",\n      \"description\": \"Gradient end color for the Space card\",\n      \"pattern\": \"^#[0-9a-fA-F]{6}$|^[a-z]+$\"\n    },\n    \"pinned\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Space is pinned on the author's profile\",\n      \"default\": false\n    },\n    \"license\": {\n      \"type\": \"string\",\n      \"description\": \"License identifier\"\n    },\n    \"short_description\": {\n      \"type\": \"string\",\n      \"description\": \"Brief description shown on the Space card\"\n    },\n    \"models\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Model IDs used by this Space\"\n    },\n    \"datasets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Dataset IDs used by this Space\"\n    },\n    \"runtime\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Runtime status and configuration\",\n      \"properties\": {\n        \"stage\": {\n          \"type\": \"string\",\n          \"description\": \"Current runtime stage\",\n          \"enum\": [\n            \"RUNNING\",\n            \"STOPPED\",\n            \"BUILDING\",\n            \"BUILD_ERROR\",\n            \"RUNTIME_ERROR\",\n            \"PAUSED\",\n            \"SLEEPING\",\n            \"DELETING\",\n            \"NO_APP_FILE\",\n            \"CONFIG_ERROR\"\n          ]\n        },\n        \"hardware\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"current\": {\n              \"type\": \"string\",\n              \"description\": \"Currently assigned hardware\",\n              \"enum\": [\n                \"cpu-basic\",\n                \"cpu-upgrade\",\n                \"t4-small\",\n                \"t4-medium\",\n                \"a10g-small\",\n                \"a10g-large\",\n \
  \               \"a10g-largex2\",\n                \"a10g-largex4\",\n                \"a100-large\",\n                \"zero-a10g\",\n                \"zero-gpu\"\n              ]\n            },\n            \"requested\": {\n              \"type\": \"string\",\n              \"description\": \"Requested hardware (may differ during scaling)\"\n            }\n          }\n        },\n        \"storage\": {\n          \"type\": \"string\",\n          \"description\": \"Persistent storage tier\",\n          \"enum\": [\n            \"small\",\n            \"medium\",\n            \"large\"\n          ]\n        },\n        \"gcTimeout\": {\n          \"type\": \"integer\",\n          \"description\": \"Garbage collection timeout in seconds\"\n        },\n        \"replicas\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"current\": {\n              \"type\": \"integer\"\n            },\n            \"requested\": {\n              \"type\": \"integer\"\n\
  \            }\n          }\n        }\n      }\n    },\n    \"siblings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"rfilename\": {\n            \"type\": \"string\",\n            \"description\": \"Relative file path\"\n          },\n          \"size\": {\n            \"type\": \"integer\",\n            \"description\": \"File size in bytes\"\n          }\n        }\n      },\n      \"description\": \"Files in the Space repository\"\n    },\n    \"cardData\": {\n      \"type\": \"object\",\n      \"description\": \"Parsed metadata from the Space card YAML front matter\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\"\n        },\n        \"emoji\": {\n          \"type\": \"string\"\n        },\n        \"colorFrom\": {\n          \"type\": \"string\"\n        },\n        \"colorTo\": {\n          \"type\": \"string\"\n        },\n        \"sdk\": {\n          \"type\": \"string\"\
  \n        },\n        \"sdk_version\": {\n          \"type\": \"string\"\n        },\n        \"app_file\": {\n          \"type\": \"string\"\n        },\n        \"pinned\": {\n          \"type\": \"boolean\"\n        },\n        \"license\": {\n          \"type\": \"string\"\n        },\n        \"models\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"datasets\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"duplicated_from\": {\n          \"type\": \"string\",\n          \"description\": \"Space this was duplicated from\"\n        },\n        \"hf_oauth\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether HF OAuth is enabled\"\n        },\n        \"hf_oauth_scopes\"\
  : {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"OAuth scopes requested\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-space-schema.json
tags: []
title: Hugging Face Space
---
