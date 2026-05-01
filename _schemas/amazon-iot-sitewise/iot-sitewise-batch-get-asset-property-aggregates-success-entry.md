---
description: Contains success information for an entry that is associated with the <a href="https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchGetAssetPropertyAggregates.html">BatchGetAssetPropertyAggregates</a> API.
layout: schema
name: BatchGetAssetPropertyAggregatesSuccessEntry
properties_list:
- description: ''
  name: entryId
  type: object
- description: ''
  name: aggregatedValues
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-get-asset-property-aggregates-success-entry-schema.json
slug: iot-sitewise-batch-get-asset-property-aggregates-success-entry
source_filename: iot-sitewise-batch-get-asset-property-aggregates-success-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-aggregates-success-entry-schema.json\",\n  \"title\": \"BatchGetAssetPropertyAggregatesSuccessEntry\",\n  \"description\": \"Contains success information for an entry that is associated with the <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchGetAssetPropertyAggregates.html\\\">BatchGetAssetPropertyAggregates</a> API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntryId\"\n        },\n        {\n          \"description\": \"The ID of the entry.\"\n        }\n      ]\n    },\n    \"aggregatedValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatedValues\"\n        },\n        {\n          \"\
  description\": \"The requested aggregated asset property values (for example, average, minimum, and maximum).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"entryId\",\n    \"aggregatedValues\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-aggregates-success-entry-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchGetAssetPropertyAggregatesSuccessEntry
---
