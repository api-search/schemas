---
description: TagResourceRequest schema from Amazon Lookout for Metrics API
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-tag-resource-request-schema.json
slug: amazon-lookout-for-metrics-tag-resource-request
source_filename: amazon-lookout-for-metrics-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"Tags to apply to the resource. Tag keys and values can contain letters, numbers, spaces, and the following symbols: <code>_.:/=+@-</code> \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-tag-resource-request-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: TagResourceRequest
---
