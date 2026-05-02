---
description: A request to generate text using an IBM watsonx.ai foundation model.
layout: schema
name: Text Generation Request
properties_list:
- description: The ID of the model to use for generation.
  name: model_id
  type: string
- description: The prompt text to send to the model.
  name: input
  type: string
- description: The watsonx.ai project ID.
  name: project_id
  type: string
- description: Generation parameters.
  name: parameters
  type: object
provider_name: International Business Machines
provider_slug: international-business-machines
schema_file: json-schema/text-generation-request.json
slug: text-generation-request
source_filename: text-generation-request.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"text-generation-request.json\",\n  \"title\": \"Text Generation Request\",\n  \"description\": \"A request to generate text using an IBM watsonx.ai foundation model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the model to use for generation.\"\n    },\n    \"input\": {\n      \"type\": \"string\",\n      \"description\": \"The prompt text to send to the model.\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"The watsonx.ai project ID.\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Generation parameters.\",\n      \"properties\": {\n        \"max_new_tokens\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of tokens to generate.\",\n          \"minimum\": 1\n        },\n        \"temperature\"\
  : {\n          \"type\": \"number\",\n          \"description\": \"Sampling temperature.\",\n          \"minimum\": 0,\n          \"maximum\": 2\n        },\n        \"top_p\": {\n          \"type\": \"number\",\n          \"description\": \"Top-p (nucleus) sampling.\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        },\n        \"top_k\": {\n          \"type\": \"integer\",\n          \"description\": \"Top-k sampling.\",\n          \"minimum\": 1\n        },\n        \"repetition_penalty\": {\n          \"type\": \"number\",\n          \"description\": \"Penalty for repeated tokens.\"\n        },\n        \"stop_sequences\": {\n          \"type\": \"array\",\n          \"description\": \"Sequences that stop generation.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"model_id\", \"input\", \"project_id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/json-schema/text-generation-request.json
tags:
- Artificial Intelligence
- Cloud
- Enterprise
- IBM
title: Text Generation Request
---
