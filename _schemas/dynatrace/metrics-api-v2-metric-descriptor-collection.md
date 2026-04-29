---
description: A paginated collection of metric descriptors returned by the list metrics endpoint.
layout: schema
name: MetricDescriptorCollection
properties_list:
- description: The cursor for the next page of results. Include this value as the nextPageKey query parameter in the next request. Null if there are no more results.
  name: nextPageKey
  type: string
- description: The total number of metrics available matching the query.
  name: totalCount
  type: integer
- description: The resolution of the data if applicable.
  name: resolution
  type: string
- description: The list of metric descriptors on this page.
  name: metrics
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/metrics-api-v2-metric-descriptor-collection-schema.json
slug: metrics-api-v2-metric-descriptor-collection
source_filename: metrics-api-v2-metric-descriptor-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/metrics-api-v2-metric-descriptor-collection-schema.json\",\n  \"title\": \"MetricDescriptorCollection\",\n  \"description\": \"A paginated collection of metric descriptors returned by the list metrics endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"The cursor for the next page of results. Include this value as the nextPageKey query parameter in the next request. Null if there are no more results.\",\n      \"nullable\": true,\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The total number of metrics available matching the query.\",\n      \"example\": 500\n    },\n    \"resolution\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The resolution of the data if applicable.\",\n      \"example\": \"example-value\"\n    },\n    \"metrics\": {\n      \"type\": \"array\",\n      \"description\": \"The list of metric descriptors on this page.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MetricDescriptor\"\n      },\n      \"example\": [\n        {\n          \"metricId\": \"abc123\",\n          \"displayName\": \"Production Service\",\n          \"description\": \"Example description.\",\n          \"unit\": \"example-value\",\n          \"dduBillable\": true,\n          \"created\": 500,\n          \"lastWritten\": 500,\n          \"entityType\": [\n            \"STANDARD\"\n          ],\n          \"aggregationTypes\": [\n            \"min\"\n          ],\n          \"dimensionDefinitions\": [\n            {\n              \"key\": \"example-value\",\n              \"name\": \"Production Service\",\n              \"type\": \"STANDARD\",\n              \"displayName\":\
  \ \"Production Service\"\n            }\n          ],\n          \"transformations\": [\n            \"example-value\"\n          ],\n          \"defaultAggregation\": {}\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/metrics-api-v2-metric-descriptor-collection-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: MetricDescriptorCollection
---
