---
description: SelectAggregateResourceConfigResponse schema
layout: schema
name: SelectAggregateResourceConfigResponse
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
schema_file: json-schema/config-select-aggregate-resource-config-response-schema.json
slug: config-select-aggregate-resource-config-response
source_filename: config-select-aggregate-resource-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-select-aggregate-resource-config-response-schema.json\",\n  \"title\": \"SelectAggregateResourceConfigResponse\",\n  \"description\": \"SelectAggregateResourceConfigResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Results\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Results\"\n        },\n        {\n          \"description\": \"Returns the results for the SQL query.\"\n        }\n      ]\n    },\n    \"QueryInfo\": {\n      \"$ref\": \"#/components/schemas/QueryInfo\"\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The nextToken string returned in a previous request that you use to request the next page of results in a paginated\
  \ response. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-select-aggregate-resource-config-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: SelectAggregateResourceConfigResponse
---
