---
description: BatchGetAssetPropertyValueErrorEntries schema
layout: schema
name: BatchGetAssetPropertyValueErrorEntries
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-get-asset-property-value-error-entries-schema.json
slug: iot-sitewise-batch-get-asset-property-value-error-entries
source_filename: iot-sitewise-batch-get-asset-property-value-error-entries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-error-entries-schema.json\",\n  \"title\": \"BatchGetAssetPropertyValueErrorEntries\",\n  \"description\": \"BatchGetAssetPropertyValueErrorEntries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"errorCode\",\n      \"errorMessage\",\n      \"entryId\"\n    ],\n    \"properties\": {\n      \"errorCode\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/BatchGetAssetPropertyValueErrorCode\"\n          },\n          {\n            \"description\": \"The error code.\"\n          }\n        ]\n      },\n      \"errorMessage\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ErrorMessage\"\n          },\n          {\n            \"description\"\
  : \"The associated error message.\"\n          }\n        ]\n      },\n      \"entryId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EntryId\"\n          },\n          {\n            \"description\": \"The ID of the entry.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains error information for an asset property value entry that is associated with the <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchGetAssetPropertyValue.html\\\">BatchGetAssetPropertyValue</a> API.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-error-entries-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchGetAssetPropertyValueErrorEntries
---
