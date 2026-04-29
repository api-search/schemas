---
description: PutAggregationAuthorizationRequest schema
layout: schema
name: PutAggregationAuthorizationRequest
properties_list:
- description: ''
  name: AuthorizedAccountId
  type: object
- description: ''
  name: AuthorizedAwsRegion
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-aggregation-authorization-request-schema.json
slug: config-put-aggregation-authorization-request
source_filename: config-put-aggregation-authorization-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-aggregation-authorization-request-schema.json\",\n  \"title\": \"PutAggregationAuthorizationRequest\",\n  \"description\": \"PutAggregationAuthorizationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuthorizedAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the account authorized to aggregate data.\"\n        }\n      ]\n    },\n    \"AuthorizedAwsRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The region authorized to collect aggregated data.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/TagsList\"\n        },\n        {\n          \"description\": \"An array of tag object.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AuthorizedAccountId\",\n    \"AuthorizedAwsRegion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-aggregation-authorization-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutAggregationAuthorizationRequest
---
