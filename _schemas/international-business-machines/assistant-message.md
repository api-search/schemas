---
description: A message exchanged with an IBM watsonx Assistant.
layout: schema
name: Assistant Message
properties_list:
- description: The user input.
  name: input
  type: object
- description: The assistant response.
  name: output
  type: object
- description: Session context data.
  name: context
  type: object
provider_name: International Business Machines
provider_slug: international-business-machines
schema_file: json-schema/assistant-message.json
slug: assistant-message
source_filename: assistant-message.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"assistant-message.json\",\n  \"title\": \"Assistant Message\",\n  \"description\": \"A message exchanged with an IBM watsonx Assistant.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"The user input.\",\n      \"properties\": {\n        \"message_type\": {\n          \"type\": \"string\",\n          \"enum\": [\"text\", \"search\"],\n          \"description\": \"The type of the message.\"\n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"The text of the user input.\"\n        },\n        \"options\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"return_context\": {\n              \"type\": \"boolean\"\n            },\n            \"debug\": {\n              \"type\": \"boolean\"\n            }\n          }\n        }\n      }\n    },\n    \"output\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"The assistant response.\",\n      \"properties\": {\n        \"generic\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"response_type\": {\n                \"type\": \"string\"\n              },\n              \"text\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"intents\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"intent\": {\n                \"type\": \"string\"\n              },\n              \"confidence\": {\n                \"type\": \"number\"\n              }\n            }\n          }\n        },\n        \"entities\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"entity\"\
  : {\n                \"type\": \"string\"\n              },\n              \"value\": {\n                \"type\": \"string\"\n              },\n              \"confidence\": {\n                \"type\": \"number\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Session context data.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/json-schema/assistant-message.json
tags:
- Artificial Intelligence
- Cloud
- Enterprise
- IBM
title: Assistant Message
---
