---
description: Schema for messages in the Jupyter kernel messaging protocol (v5.4). All messages exchanged between frontends and kernels follow this envelope structure.
layout: schema
name: Jupyter Kernel Message
properties_list:
- description: ''
  name: header
  type: object
- description: Header of the parent message this is a reply to. Empty object for initial requests.
  name: parent_header
  type: object
- description: Message metadata.
  name: metadata
  type: object
- description: The message content. Structure varies by msg_type.
  name: content
  type: object
- description: Optional binary buffers for the message.
  name: buffers
  type: array
- description: The messaging channel (used when multiplexed over WebSocket).
  name: channel
  type: string
provider_name: Jupyter Notebook
provider_slug: jupyter-notebook
schema_file: json-schema/jupyter-kernel-message.json
slug: jupyter-kernel-message
source_filename: jupyter-kernel-message.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"jupyter-kernel-message.json\",\n  \"title\": \"Jupyter Kernel Message\",\n  \"description\": \"Schema for messages in the Jupyter kernel messaging protocol (v5.4). All messages exchanged between frontends and kernels follow this envelope structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"header\": {\n      \"$ref\": \"#/$defs/MessageHeader\"\n    },\n    \"parent_header\": {\n      \"description\": \"Header of the parent message this is a reply to. Empty object for initial requests.\",\n      \"oneOf\": [\n        {\"$ref\": \"#/$defs/MessageHeader\"},\n        {\"type\": \"object\", \"maxProperties\": 0}\n      ]\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Message metadata.\",\n      \"additionalProperties\": true\n    },\n    \"content\": {\n      \"type\": \"object\",\n      \"description\": \"The message content. Structure varies by msg_type.\"\
  ,\n      \"additionalProperties\": true\n    },\n    \"buffers\": {\n      \"type\": \"array\",\n      \"description\": \"Optional binary buffers for the message.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"contentEncoding\": \"base64\"\n      }\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"description\": \"The messaging channel (used when multiplexed over WebSocket).\",\n      \"enum\": [\"shell\", \"iopub\", \"stdin\", \"control\"]\n    }\n  },\n  \"required\": [\"header\", \"parent_header\", \"metadata\", \"content\"],\n  \"$defs\": {\n    \"MessageHeader\": {\n      \"type\": \"object\",\n      \"description\": \"The header of a Jupyter kernel message.\",\n      \"properties\": {\n        \"msg_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique message identifier (typically a UUID).\"\n        },\n        \"msg_type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of message.\",\n      \
  \    \"enum\": [\n            \"execute_request\",\n            \"execute_reply\",\n            \"execute_input\",\n            \"execute_result\",\n            \"inspect_request\",\n            \"inspect_reply\",\n            \"complete_request\",\n            \"complete_reply\",\n            \"history_request\",\n            \"history_reply\",\n            \"is_complete_request\",\n            \"is_complete_reply\",\n            \"kernel_info_request\",\n            \"kernel_info_reply\",\n            \"shutdown_request\",\n            \"shutdown_reply\",\n            \"interrupt_request\",\n            \"interrupt_reply\",\n            \"debug_request\",\n            \"debug_reply\",\n            \"debug_event\",\n            \"input_request\",\n            \"input_reply\",\n            \"stream\",\n            \"display_data\",\n            \"update_display_data\",\n            \"error\",\n            \"status\",\n            \"clear_output\",\n            \"comm_open\",\n        \
  \    \"comm_msg\",\n            \"comm_close\",\n            \"comm_info_request\",\n            \"comm_info_reply\"\n          ]\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"Username associated with the message.\"\n        },\n        \"session\": {\n          \"type\": \"string\",\n          \"description\": \"Session identifier (typically a UUID).\"\n        },\n        \"date\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the message was created.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Messaging protocol version.\",\n          \"pattern\": \"^\\\\d+\\\\.\\\\d+$\"\n        }\n      },\n      \"required\": [\"msg_id\", \"msg_type\", \"username\", \"session\", \"date\", \"version\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/json-schema/jupyter-kernel-message.json
tags:
- Data Science
- Interactive Computing
- Jupyter
- Machine Learning
- Notebooks
- Python
title: Jupyter Kernel Message
---
