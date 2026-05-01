---
description: SelectResourceConfigRequest schema
layout: schema
name: SelectResourceConfigRequest
properties_list:
- description: ''
  name: Expression
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-select-resource-config-request-schema.json
slug: config-select-resource-config-request
source_filename: config-select-resource-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-select-resource-config-request-schema.json\",\n  \"title\": \"SelectResourceConfigRequest\",\n  \"description\": \"SelectResourceConfigRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Expression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Expression\"\n        },\n        {\n          \"description\": \"The SQL query <code>SELECT</code> command.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of query results returned on each page. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n     \
  \   {\n          \"description\": \"The <code>nextToken</code> string returned in a previous request that you use to request the next page of results in a paginated response. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Expression\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-select-resource-config-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: SelectResourceConfigRequest
---
