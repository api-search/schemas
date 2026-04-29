---
description: Contains error details for the requested associate project asset action.
layout: schema
name: AssetErrorDetails
properties_list:
- description: ''
  name: assetId
  type: object
- description: ''
  name: code
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-error-details-schema.json
slug: iot-sitewise-asset-error-details
source_filename: iot-sitewise-asset-error-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-error-details-schema.json\",\n  \"title\": \"AssetErrorDetails\",\n  \"description\": \"Contains error details for the requested associate project asset action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the asset.\"\n        }\n      ]\n    },\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetErrorCode\"\n        },\n        {\n          \"description\": \"The error code.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetErrorMessage\"\n        },\n        {\n          \"description\": \"\
  The error message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"assetId\",\n    \"code\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-error-details-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetErrorDetails
---
