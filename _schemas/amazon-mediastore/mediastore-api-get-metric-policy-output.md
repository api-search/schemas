---
description: GetMetricPolicyOutput schema from Amazon MediaStore API
layout: schema
name: GetMetricPolicyOutput
properties_list:
- description: ''
  name: MetricPolicy
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-get-metric-policy-output-schema.json
slug: mediastore-api-get-metric-policy-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-get-metric-policy-output-schema.json\",\n  \"title\": \"GetMetricPolicyOutput\",\n  \"description\": \"GetMetricPolicyOutput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricPolicy\"\n        },\n        {\n          \"description\": \"The metric policy that is associated with the specific container.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MetricPolicy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-get-metric-policy-output-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: GetMetricPolicyOutput
---
