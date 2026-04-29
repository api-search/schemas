---
description: DeleteResourcePolicyRequest schema from Amazon X-Ray API
layout: schema
name: DeleteResourcePolicyRequest
properties_list:
- description: ''
  name: PolicyName
  type: object
- description: ''
  name: PolicyRevisionId
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-delete-resource-policy-request-schema.json
slug: xray-delete-resource-policy-request
source_filename: xray-delete-resource-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"PolicyName\"\n  ],\n  \"title\": \"DeleteResourcePolicyRequest\",\n  \"properties\": {\n    \"PolicyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyName\"\n        },\n        {\n          \"description\": \"The name of the resource policy to delete.\"\n        }\n      ]\n    },\n    \"PolicyRevisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyRevisionId\"\n        },\n        {\n          \"description\": \"Specifies a specific policy revision to delete. Provide a <code>PolicyRevisionId</code> to ensure an atomic delete operation. If the provided revision id does not match the latest policy revision id, an <code>InvalidPolicyRevisionIdException</code> exception is returned. \"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-delete-resource-policy-request-schema.json\"\
  ,\n  \"description\": \"DeleteResourcePolicyRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-delete-resource-policy-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: DeleteResourcePolicyRequest
---
