---
description: A list of EC2 instance IDs corresponding to the segments in a trace.
layout: schema
name: InstanceIdDetail
properties_list:
- description: ''
  name: Id
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-instance-id-detail-schema.json
slug: xray-instance-id-detail
source_filename: xray-instance-id-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID of a corresponding EC2 instance.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A list of EC2 instance IDs corresponding to the segments in a trace. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstanceIdDetail\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-instance-id-detail-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-instance-id-detail-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: InstanceIdDetail
---
