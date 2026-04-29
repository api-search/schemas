---
description: LLM text completion request.
layout: schema
name: CompleteRequest
properties_list:
- description: The model name. See documentation for possible values.
  name: model
  type: string
- description: ''
  name: messages
  type: array
- description: Temperature controls the amount of randomness used in response generation. A higher temperature corresponds to more randomness.
  name: temperature
  type: number
- description: Threshold probability for nucleus sampling. A higher top-p value increases the diversity of tokens that the model considers, while a lower value results in more predictable output.
  name: top_p
  type: number
- description: The maximum number of output tokens to produce. The default value is model-dependent.
  name: max_tokens
  type: integer
- description: Deprecated in favor of "max_tokens", which has identical behavior.
  name: max_output_tokens
  type: integer
- description: An object describing response format config for structured-output mode.
  name: response_format
  type: object
- description: List of tools to be used during tool calling
  name: tools
  type: array
- description: The provisioned throughput ID to be used with the request.
  name: provisioned_throughput_id
  type: string
- description: Reserved
  name: sf-ml-xp-inflight-prompt-action
  type: string
- description: Reserved
  name: sf-ml-xp-inflight-prompt-client-id
  type: string
- description: Reserved
  name: sf-ml-xp-inflight-prompt-public-key
  type: string
- description: Reserved
  name: stream
  type: boolean
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-inference-complete-request-schema.json
slug: cortex-inference-complete-request
source_filename: cortex-inference-complete-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompleteRequest\",\n  \"type\": \"object\",\n  \"description\": \"LLM text completion request.\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model name. See documentation for possible values.\"\n    },\n    \"messages\": {\n      \"type\": \"array\"\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"description\": \"Temperature controls the amount of randomness used in response generation. A higher temperature corresponds to more randomness.\"\n    },\n    \"top_p\": {\n      \"type\": \"number\",\n      \"description\": \"Threshold probability for nucleus sampling. A higher top-p value increases the diversity of tokens that the model considers, while a lower value results in more predictable output.\"\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of output tokens\
  \ to produce. The default value is model-dependent.\"\n    },\n    \"max_output_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Deprecated in favor of \\\"max_tokens\\\", which has identical behavior.\"\n    },\n    \"response_format\": {\n      \"type\": \"object\",\n      \"description\": \"An object describing response format config for structured-output mode.\"\n    },\n    \"tools\": {\n      \"type\": \"array\",\n      \"description\": \"List of tools to be used during tool calling\"\n    },\n    \"provisioned_throughput_id\": {\n      \"type\": \"string\",\n      \"description\": \"The provisioned throughput ID to be used with the request.\"\n    },\n    \"sf-ml-xp-inflight-prompt-action\": {\n      \"type\": \"string\",\n      \"description\": \"Reserved\"\n    },\n    \"sf-ml-xp-inflight-prompt-client-id\": {\n      \"type\": \"string\",\n      \"description\": \"Reserved\"\n    },\n    \"sf-ml-xp-inflight-prompt-public-key\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Reserved\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\",\n      \"description\": \"Reserved\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-inference-complete-request-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: CompleteRequest
---
