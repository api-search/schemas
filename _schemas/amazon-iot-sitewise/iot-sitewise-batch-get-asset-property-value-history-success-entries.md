---
description: BatchGetAssetPropertyValueHistorySuccessEntries schema
layout: schema
name: BatchGetAssetPropertyValueHistorySuccessEntries
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-get-asset-property-value-history-success-entries-schema.json
slug: iot-sitewise-batch-get-asset-property-value-history-success-entries
source_filename: iot-sitewise-batch-get-asset-property-value-history-success-entries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-history-success-entries-schema.json\",\n  \"title\": \"BatchGetAssetPropertyValueHistorySuccessEntries\",\n  \"description\": \"BatchGetAssetPropertyValueHistorySuccessEntries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"entryId\",\n      \"assetPropertyValueHistory\"\n    ],\n    \"properties\": {\n      \"entryId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EntryId\"\n          },\n          {\n            \"description\": \"The ID of the entry.\"\n          }\n        ]\n      },\n      \"assetPropertyValueHistory\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AssetPropertyValueHistory\"\n          },\n         \
  \ {\n            \"description\": \"The requested historical values for the specified asset property.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains success information for an entry that is associated with the <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchGetAssetPropertyValue.html\\\">BatchGetAssetPropertyValueHistory</a> API.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-history-success-entries-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchGetAssetPropertyValueHistorySuccessEntries
---
