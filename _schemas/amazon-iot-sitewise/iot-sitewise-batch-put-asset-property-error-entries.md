---
description: BatchPutAssetPropertyErrorEntries schema
layout: schema
name: BatchPutAssetPropertyErrorEntries
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-put-asset-property-error-entries-schema.json
slug: iot-sitewise-batch-put-asset-property-error-entries
source_filename: iot-sitewise-batch-put-asset-property-error-entries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-put-asset-property-error-entries-schema.json\",\n  \"title\": \"BatchPutAssetPropertyErrorEntries\",\n  \"description\": \"BatchPutAssetPropertyErrorEntries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"entryId\",\n      \"errors\"\n    ],\n    \"properties\": {\n      \"entryId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EntryId\"\n          },\n          {\n            \"description\": \"The ID of the failed entry.\"\n          }\n        ]\n      },\n      \"errors\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/BatchPutAssetPropertyErrors\"\n          },\n          {\n            \"description\": \"The list of update property value errors.\"\
  \n          }\n        ]\n      }\n    },\n    \"description\": \"Contains error information for asset property value entries that are associated with the <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchPutAssetPropertyValue.html\\\">BatchPutAssetPropertyValue</a> API.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-put-asset-property-error-entries-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchPutAssetPropertyErrorEntries
---
