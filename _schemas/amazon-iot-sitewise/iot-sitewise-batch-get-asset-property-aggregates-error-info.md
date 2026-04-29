---
description: Contains the error code and the timestamp for an asset property aggregate entry that is associated with the <a href="https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchGetAssetPropertyAggregates.html">BatchGetAssetPropertyAggregates</a> API.
layout: schema
name: BatchGetAssetPropertyAggregatesErrorInfo
properties_list:
- description: ''
  name: errorCode
  type: object
- description: ''
  name: errorTimestamp
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-get-asset-property-aggregates-error-info-schema.json
slug: iot-sitewise-batch-get-asset-property-aggregates-error-info
source_filename: iot-sitewise-batch-get-asset-property-aggregates-error-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-aggregates-error-info-schema.json\",\n  \"title\": \"BatchGetAssetPropertyAggregatesErrorInfo\",\n  \"description\": \"Contains the error code and the timestamp for an asset property aggregate entry that is associated with the <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchGetAssetPropertyAggregates.html\\\">BatchGetAssetPropertyAggregates</a> API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetAssetPropertyAggregatesErrorCode\"\n        },\n        {\n          \"description\": \"The error code.\"\n        }\n      ]\n    },\n    \"errorTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The date the error occurred, in Unix epoch time.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"errorCode\",\n    \"errorTimestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-aggregates-error-info-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchGetAssetPropertyAggregatesErrorInfo
---
