---
description: Contains success information for an entry that is associated with the <a href="https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchGetAssetPropertyValue.html">BatchGetAssetPropertyValue</a> API.
layout: schema
name: BatchGetAssetPropertyValueSuccessEntry
properties_list:
- description: ''
  name: entryId
  type: object
- description: Contains asset property value information.
  name: assetPropertyValue
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-get-asset-property-value-success-entry-schema.json
slug: iot-sitewise-batch-get-asset-property-value-success-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-success-entry-schema.json\",\n  \"title\": \"BatchGetAssetPropertyValueSuccessEntry\",\n  \"description\": \"Contains success information for an entry that is associated with the <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchGetAssetPropertyValue.html\\\">BatchGetAssetPropertyValue</a> API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntryId\"\n        },\n        {\n          \"description\": \"The ID of the entry.\"\n        }\n      ]\n    },\n    \"assetPropertyValue\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"value\",\n        \"timestamp\"\n      ],\n      \"properties\": {\n        \"value\"\
  : {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Variant\"\n            },\n            {\n              \"description\": \"The value of the asset property (see <code>Variant</code>).\"\n            }\n          ]\n        },\n        \"timestamp\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/TimeInNanos\"\n            },\n            {\n              \"description\": \"The timestamp of the asset property value.\"\n            }\n          ]\n        },\n        \"quality\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Quality\"\n            },\n            {\n              \"description\": \"The quality of the asset property value.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Contains asset property value information.\"\n    }\n  },\n  \"required\": [\n    \"entryId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-success-entry-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchGetAssetPropertyValueSuccessEntry
---
