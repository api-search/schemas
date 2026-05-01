---
description: Specifies the status of advanced security options for the specified Elasticsearch domain.
layout: schema
name: AdvancedSecurityOptionsStatus
properties_list:
- description: ''
  name: Options
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-advanced-security-options-status-schema.json
slug: openapi-advanced-security-options-status
source_filename: openapi-advanced-security-options-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-advanced-security-options-status-schema.json\",\n  \"title\": \"AdvancedSecurityOptionsStatus\",\n  \"description\": \" Specifies the status of advanced security options for the specified Elasticsearch domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Options\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdvancedSecurityOptions\"\n        },\n        {\n          \"description\": \" Specifies advanced security options for the specified Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionStatus\"\n        },\n        {\n          \"description\": \" Status of the advanced security options for the specified Elasticsearch domain.\"\n        }\n     \
  \ ]\n    }\n  },\n  \"required\": [\n    \"Options\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-advanced-security-options-status-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: AdvancedSecurityOptionsStatus
---
