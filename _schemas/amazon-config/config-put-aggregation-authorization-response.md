---
description: PutAggregationAuthorizationResponse schema
layout: schema
name: PutAggregationAuthorizationResponse
properties_list:
- description: ''
  name: AggregationAuthorization
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-aggregation-authorization-response-schema.json
slug: config-put-aggregation-authorization-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-aggregation-authorization-response-schema.json\",\n  \"title\": \"PutAggregationAuthorizationResponse\",\n  \"description\": \"PutAggregationAuthorizationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AggregationAuthorization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationAuthorization\"\n        },\n        {\n          \"description\": \"Returns an AggregationAuthorization object. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-aggregation-authorization-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutAggregationAuthorizationResponse
---
