---
description: Contains information for an entry that has been processed by the previous <a href="https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchGetAssetPropertyValue.html">BatchGetAssetPropertyValueHistory</a> request.
layout: schema
name: BatchGetAssetPropertyValueHistorySkippedEntry
properties_list:
- description: ''
  name: entryId
  type: object
- description: ''
  name: completionStatus
  type: object
- description: ''
  name: errorInfo
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-get-asset-property-value-history-skipped-entry-schema.json
slug: iot-sitewise-batch-get-asset-property-value-history-skipped-entry
source_filename: iot-sitewise-batch-get-asset-property-value-history-skipped-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-history-skipped-entry-schema.json\",\n  \"title\": \"BatchGetAssetPropertyValueHistorySkippedEntry\",\n  \"description\": \"Contains information for an entry that has been processed by the previous <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchGetAssetPropertyValue.html\\\">BatchGetAssetPropertyValueHistory</a> request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntryId\"\n        },\n        {\n          \"description\": \"The ID of the entry.\"\n        }\n      ]\n    },\n    \"completionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchEntryCompletionStatus\"\n        },\n  \
  \      {\n          \"description\": \"The completion status of each entry that is associated with the <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchGetAssetPropertyValueHistory.html\\\">BatchGetAssetPropertyValueHistory</a> API.\"\n        }\n      ]\n    },\n    \"errorInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetAssetPropertyValueHistoryErrorInfo\"\n        },\n        {\n          \"description\": \"The error information, such as the error code and the timestamp.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"entryId\",\n    \"completionStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-history-skipped-entry-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchGetAssetPropertyValueHistorySkippedEntry
---
