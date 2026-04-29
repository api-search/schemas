---
description: The output for the <a>GetResourceConfigHistory</a> action.
layout: schema
name: GetResourceConfigHistoryResponse
properties_list:
- description: ''
  name: configurationItems
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-resource-config-history-response-schema.json
slug: config-get-resource-config-history-response
source_filename: config-get-resource-config-history-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-resource-config-history-response-schema.json\",\n  \"title\": \"GetResourceConfigHistoryResponse\",\n  \"description\": \"The output for the <a>GetResourceConfigHistory</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationItems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationItemList\"\n        },\n        {\n          \"description\": \"A list that contains the configuration history of one or more resources.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that you use in a subsequent request to get the next page of results in a paginated response.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-resource-config-history-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetResourceConfigHistoryResponse
---
