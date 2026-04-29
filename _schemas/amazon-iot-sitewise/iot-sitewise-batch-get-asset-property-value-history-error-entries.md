---
description: BatchGetAssetPropertyValueHistoryErrorEntries schema
layout: schema
name: BatchGetAssetPropertyValueHistoryErrorEntries
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-get-asset-property-value-history-error-entries-schema.json
slug: iot-sitewise-batch-get-asset-property-value-history-error-entries
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-history-error-entries-schema.json\",\n  \"title\": \"BatchGetAssetPropertyValueHistoryErrorEntries\",\n  \"description\": \"BatchGetAssetPropertyValueHistoryErrorEntries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"errorCode\",\n      \"errorMessage\",\n      \"entryId\"\n    ],\n    \"properties\": {\n      \"errorCode\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/BatchGetAssetPropertyValueHistoryErrorCode\"\n          },\n          {\n            \"description\": \"The error code.\"\n          }\n        ]\n      },\n      \"errorMessage\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ErrorMessage\"\n          },\n\
  \          {\n            \"description\": \"The associated error message.\"\n          }\n        ]\n      },\n      \"entryId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EntryId\"\n          },\n          {\n            \"description\": \"The ID of the entry.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A list of the errors (if any) associated with the batch request. Each error entry contains the <code>entryId</code> of the entry that failed.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-history-error-entries-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchGetAssetPropertyValueHistoryErrorEntries
---
