---
description: SegmentationResult schema from Amplitude Dashboard REST API
layout: schema
name: SegmentationResult
properties_list:
- description: ''
  name: data
  type: object
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/dashboard-rest-api-segmentation-result-schema.json
slug: dashboard-rest-api-segmentation-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dashboard-rest-api-segmentation-result-schema.json\",\n  \"title\": \"SegmentationResult\",\n  \"description\": \"SegmentationResult schema from Amplitude Dashboard REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"series\": {\n          \"type\": \"array\",\n          \"description\": \"An array of data series, one per segment or group-by value.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"additionalProperties\": true\n          }\n        },\n        \"seriesLabels\": {\n          \"type\": \"array\",\n          \"description\": \"Labels corresponding to each series.\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\
  \n            }\n          }\n        },\n        \"xValues\": {\n          \"type\": \"array\",\n          \"description\": \"The x-axis values representing time periods.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dashboard-rest-api-segmentation-result-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: SegmentationResult
---
