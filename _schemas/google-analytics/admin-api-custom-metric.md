---
description: A definition for a custom metric.
layout: schema
name: CustomMetric
properties_list:
- description: Optional. Description for this custom dimension. Max length of 150 characters.
  name: description
  type: string
- description: 'Required. Display name for this custom metric as shown in the Analytics UI. Max length of 82 characters, alphanumeric plus space and underscore starting with a letter. Legacy system-generated display '
  name: displayName
  type: string
- description: Required. The type for the custom metric's value.
  name: measurementUnit
  type: string
- description: 'Output only. Resource name for this CustomMetric resource. Format: properties/{property}/customMetrics/{customMetric}'
  name: name
  type: string
- description: Required. Immutable. Tagging name for this custom metric. If this is an event-scoped metric, then this is the event parameter name. May only contain alphanumeric and underscore charactes, starting wit
  name: parameterName
  type: string
- description: Optional. Types of restricted data that this metric may contain. Required for metrics with CURRENCY measurement unit. Must be empty for metrics with a non-CURRENCY measurement unit.
  name: restrictedMetricType
  type: array
- description: Required. Immutable. The scope of this custom metric.
  name: scope
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/admin-api-custom-metric-schema.json
slug: admin-api-custom-metric
source_filename: admin-api-custom-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-custom-metric-schema.json\",\n  \"title\": \"CustomMetric\",\n  \"description\": \"A definition for a custom metric.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Optional. Description for this custom dimension. Max length of 150 characters.\",\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"description\": \"Required. Display name for this custom metric as shown in the Analytics UI. Max length of 82 characters, alphanumeric plus space and underscore starting with a letter. Legacy system-generated display names may contain square brackets, but updates to this field will never permit square brackets.\",\n      \"type\": \"string\"\n    },\n    \"measurementUnit\": {\n      \"description\": \"Required. The type for the custom\
  \ metric's value.\",\n      \"enum\": [\n        \"MEASUREMENT_UNIT_UNSPECIFIED\",\n        \"STANDARD\",\n        \"CURRENCY\",\n        \"FEET\",\n        \"METERS\",\n        \"KILOMETERS\",\n        \"MILES\",\n        \"MILLISECONDS\",\n        \"SECONDS\",\n        \"MINUTES\",\n        \"HOURS\"\n      ],\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Output only. Resource name for this CustomMetric resource. Format: properties/{property}/customMetrics/{customMetric}\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"parameterName\": {\n      \"description\": \"Required. Immutable. Tagging name for this custom metric. If this is an event-scoped metric, then this is the event parameter name. May only contain alphanumeric and underscore charactes, starting with a letter. Max length of 40 characters for event-scoped metrics.\",\n      \"type\": \"string\"\n    },\n    \"restrictedMetricType\": {\n      \"description\": \"Optional.\
  \ Types of restricted data that this metric may contain. Required for metrics with CURRENCY measurement unit. Must be empty for metrics with a non-CURRENCY measurement unit.\",\n      \"items\": {\n        \"enum\": [\n          \"RESTRICTED_METRIC_TYPE_UNSPECIFIED\",\n          \"COST_DATA\",\n          \"REVENUE_DATA\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"scope\": {\n      \"description\": \"Required. Immutable. The scope of this custom metric.\",\n      \"enum\": [\n        \"METRIC_SCOPE_UNSPECIFIED\",\n        \"EVENT\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-custom-metric-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: CustomMetric
---
