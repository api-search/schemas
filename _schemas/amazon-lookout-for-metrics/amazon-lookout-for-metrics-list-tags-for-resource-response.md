---
description: ListTagsForResourceResponse schema from Amazon Lookout for Metrics API
layout: schema
name: ListTagsForResourceResponse
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-list-tags-for-resource-response-schema.json
slug: amazon-lookout-for-metrics-list-tags-for-resource-response
source_filename: amazon-lookout-for-metrics-list-tags-for-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-tags-for-resource-response-schema.json\",\n  \"title\": \"ListTagsForResourceResponse\",\n  \"description\": \"ListTagsForResourceResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The resource's tags.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-tags-for-resource-response-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: ListTagsForResourceResponse
---
