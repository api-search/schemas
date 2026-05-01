---
description: Specifies metric-based criteria for including or excluding endpoints from a segment. These criteria derive from custom metrics that you define for endpoints.
layout: schema
name: MetricDimension
properties_list:
- description: ''
  name: ComparisonOperator
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-metric-dimension-schema.json
slug: amazon-pinpoint-metric-dimension
source_filename: amazon-pinpoint-metric-dimension-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-metric-dimension-schema.json\",\n  \"title\": \"MetricDimension\",\n  \"description\": \"Specifies metric-based criteria for including or excluding endpoints from a segment. These criteria derive from custom metrics that you define for endpoints.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ComparisonOperator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The operator to use when comparing metric values. Valid values are: GREATER_THAN, LESS_THAN, GREATER_THAN_OR_EQUAL, LESS_THAN_OR_EQUAL, and EQUAL.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"description\"\
  : \"The value to compare.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ComparisonOperator\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-metric-dimension-schema.json
tags:
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: MetricDimension
---
