---
description: GetMetricPolicyInput schema from Amazon MediaStore API
layout: schema
name: GetMetricPolicyInput
properties_list:
- description: ''
  name: ContainerName
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-get-metric-policy-input-schema.json
slug: mediastore-api-get-metric-policy-input
source_filename: mediastore-api-get-metric-policy-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-get-metric-policy-input-schema.json\",\n  \"title\": \"GetMetricPolicyInput\",\n  \"description\": \"GetMetricPolicyInput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContainerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerName\"\n        },\n        {\n          \"description\": \"The name of the container that is associated with the metric policy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ContainerName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-get-metric-policy-input-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: GetMetricPolicyInput
---
