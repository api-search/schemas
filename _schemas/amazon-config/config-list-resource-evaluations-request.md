---
description: ListResourceEvaluationsRequest schema
layout: schema
name: ListResourceEvaluationsRequest
properties_list:
- description: ''
  name: Filters
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-list-resource-evaluations-request-schema.json
slug: config-list-resource-evaluations-request
source_filename: config-list-resource-evaluations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-resource-evaluations-request-schema.json\",\n  \"title\": \"ListResourceEvaluationsRequest\",\n  \"description\": \"ListResourceEvaluationsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceEvaluationFilters\"\n        },\n        {\n          \"description\": \"Returns a <code>ResourceEvaluationFilters</code> object.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListResourceEvaluationsPageItemLimit\"\n        },\n        {\n          \"description\": \"The maximum number of evaluations returned on each page. The default is 10. You cannot specify a number greater than 100. If you specify 0, Config uses\
  \ the default.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-resource-evaluations-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ListResourceEvaluationsRequest
---
