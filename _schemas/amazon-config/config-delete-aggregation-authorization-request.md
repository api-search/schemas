---
description: DeleteAggregationAuthorizationRequest schema
layout: schema
name: DeleteAggregationAuthorizationRequest
properties_list:
- description: ''
  name: AuthorizedAccountId
  type: object
- description: ''
  name: AuthorizedAwsRegion
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delete-aggregation-authorization-request-schema.json
slug: config-delete-aggregation-authorization-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-aggregation-authorization-request-schema.json\",\n  \"title\": \"DeleteAggregationAuthorizationRequest\",\n  \"description\": \"DeleteAggregationAuthorizationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuthorizedAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the account authorized to aggregate data.\"\n        }\n      ]\n    },\n    \"AuthorizedAwsRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The region authorized to collect aggregated data.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AuthorizedAccountId\",\n\
  \    \"AuthorizedAwsRegion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-aggregation-authorization-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DeleteAggregationAuthorizationRequest
---
