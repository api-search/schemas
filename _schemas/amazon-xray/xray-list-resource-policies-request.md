---
description: ListResourcePoliciesRequest schema from Amazon X-Ray API
layout: schema
name: ListResourcePoliciesRequest
properties_list:
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-list-resource-policies-request-schema.json
slug: xray-list-resource-policies-request
source_filename: xray-list-resource-policies-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"ListResourcePoliciesRequest\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourcePolicyNextToken\"\n        },\n        {\n          \"description\": \"Not currently supported.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-list-resource-policies-request-schema.json\",\n  \"description\": \"ListResourcePoliciesRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-list-resource-policies-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: ListResourcePoliciesRequest
---
