---
description: A list of resources ARNs corresponding to the segments in a trace.
layout: schema
name: ResourceARNDetail
properties_list:
- description: ''
  name: ARN
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-resource-arn-detail-schema.json
slug: xray-resource-arn-detail
source_filename: xray-resource-arn-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ARN of a corresponding resource.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A list of resources ARNs corresponding to the segments in a trace.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourceARNDetail\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-resource-arn-detail-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-resource-arn-detail-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: ResourceARNDetail
---
