---
description: ListResourceEvaluationsResponse schema
layout: schema
name: ListResourceEvaluationsResponse
properties_list:
- description: ''
  name: ResourceEvaluations
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-list-resource-evaluations-response-schema.json
slug: config-list-resource-evaluations-response
source_filename: config-list-resource-evaluations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-resource-evaluations-response-schema.json\",\n  \"title\": \"ListResourceEvaluationsResponse\",\n  \"description\": \"ListResourceEvaluationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceEvaluations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceEvaluations\"\n        },\n        {\n          \"description\": \"Returns a <code>ResourceEvaluations</code> object.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-resource-evaluations-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ListResourceEvaluationsResponse
---
