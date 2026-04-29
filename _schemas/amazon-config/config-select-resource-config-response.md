---
description: SelectResourceConfigResponse schema
layout: schema
name: SelectResourceConfigResponse
properties_list:
- description: ''
  name: Results
  type: object
- description: ''
  name: QueryInfo
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-select-resource-config-response-schema.json
slug: config-select-resource-config-response
source_filename: config-select-resource-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-select-resource-config-response-schema.json\",\n  \"title\": \"SelectResourceConfigResponse\",\n  \"description\": \"SelectResourceConfigResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Results\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Results\"\n        },\n        {\n          \"description\": \"Returns the results for the SQL query.\"\n        }\n      ]\n    },\n    \"QueryInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryInfo\"\n        },\n        {\n          \"description\": \"Returns the <code>QueryInfo</code> object.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"\
  description\": \"The <code>nextToken</code> string returned in a previous request that you use to request the next page of results in a paginated response. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-select-resource-config-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: SelectResourceConfigResponse
---
