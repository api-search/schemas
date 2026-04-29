---
description: ListResourcePoliciesResult schema from Amazon X-Ray API
layout: schema
name: ListResourcePoliciesResult
properties_list:
- description: ''
  name: ResourcePolicies
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-list-resource-policies-result-schema.json
slug: xray-list-resource-policies-result
source_filename: xray-list-resource-policies-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourcePolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourcePolicyList\"\n        },\n        {\n          \"description\": \"The list of resource policies in the target Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourcePolicyNextToken\"\n        },\n        {\n          \"description\": \"Pagination token. Not currently supported.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListResourcePoliciesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-list-resource-policies-result-schema.json\",\n  \"description\": \"ListResourcePoliciesResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-list-resource-policies-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: ListResourcePoliciesResult
---
