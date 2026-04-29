---
description: FunctionEnvelope resource specific properties
layout: schema
name: FunctionEnvelopeProperties
properties_list:
- description: Function App ID.
  name: function_app_id
  type: string
- description: Script root path URI.
  name: script_root_path_href
  type: string
- description: Script URI.
  name: script_href
  type: string
- description: Config URI.
  name: config_href
  type: string
- description: Test data URI.
  name: test_data_href
  type: string
- description: Secrets file URI.
  name: secrets_file_href
  type: string
- description: Function URI.
  name: href
  type: string
- description: Config information.
  name: config
  type: object
- description: File list.
  name: files
  type: object
- description: Test data used when testing via the Azure Portal.
  name: test_data
  type: string
- description: The invocation URL
  name: invoke_url_template
  type: string
- description: The function language
  name: language
  type: string
- description: Gets or sets a value indicating whether the function is disabled
  name: isDisabled
  type: boolean
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-function-envelope-properties-schema.json
slug: azure-functions-function-envelope-properties
source_filename: azure-functions-function-envelope-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-function-envelope-properties-schema.json\",\n  \"title\": \"FunctionEnvelopeProperties\",\n  \"description\": \"FunctionEnvelope resource specific properties\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"function_app_id\": {\n      \"type\": \"string\",\n      \"description\": \"Function App ID.\",\n      \"x-ms-client-name\": \"functionAppId\"\n    },\n    \"script_root_path_href\": {\n      \"type\": \"string\",\n      \"description\": \"Script root path URI.\",\n      \"x-ms-client-name\": \"scriptRootPathHref\"\n    },\n    \"script_href\": {\n      \"type\": \"string\",\n      \"description\": \"Script URI.\",\n      \"x-ms-client-name\": \"scriptHref\"\n    },\n    \"config_href\": {\n      \"type\": \"string\",\n      \"description\": \"Config URI.\",\n      \"\
  x-ms-client-name\": \"configHref\"\n    },\n    \"test_data_href\": {\n      \"type\": \"string\",\n      \"description\": \"Test data URI.\",\n      \"x-ms-client-name\": \"testDataHref\"\n    },\n    \"secrets_file_href\": {\n      \"type\": \"string\",\n      \"description\": \"Secrets file URI.\",\n      \"x-ms-client-name\": \"secretsFileHref\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"Function URI.\"\n    },\n    \"config\": {\n      \"description\": \"Config information.\"\n    },\n    \"files\": {\n      \"type\": \"object\",\n      \"description\": \"File list.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"test_data\": {\n      \"type\": \"string\",\n      \"description\": \"Test data used when testing via the Azure Portal.\",\n      \"x-ms-client-name\": \"testData\"\n    },\n    \"invoke_url_template\": {\n      \"type\": \"string\",\n      \"description\": \"The invocation URL\",\n      \"x-ms-client-name\"\
  : \"invokeUrlTemplate\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"The function language\"\n    },\n    \"isDisabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Gets or sets a value indicating whether the function is disabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-function-envelope-properties-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: FunctionEnvelopeProperties
---
