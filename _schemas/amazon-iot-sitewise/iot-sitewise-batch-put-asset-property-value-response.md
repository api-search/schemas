---
description: BatchPutAssetPropertyValueResponse schema
layout: schema
name: BatchPutAssetPropertyValueResponse
properties_list:
- description: ''
  name: errorEntries
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-put-asset-property-value-response-schema.json
slug: iot-sitewise-batch-put-asset-property-value-response
source_filename: iot-sitewise-batch-put-asset-property-value-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-put-asset-property-value-response-schema.json\",\n  \"title\": \"BatchPutAssetPropertyValueResponse\",\n  \"description\": \"BatchPutAssetPropertyValueResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchPutAssetPropertyErrorEntries\"\n        },\n        {\n          \"description\": \"A list of the errors (if any) associated with the batch put request. Each error entry contains the <code>entryId</code> of the entry that failed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"errorEntries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-put-asset-property-value-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchPutAssetPropertyValueResponse
---
