---
description: BatchDisassociateProjectAssetsErrors schema
layout: schema
name: BatchDisassociateProjectAssetsErrors
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-disassociate-project-assets-errors-schema.json
slug: iot-sitewise-batch-disassociate-project-assets-errors
source_filename: iot-sitewise-batch-disassociate-project-assets-errors-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-disassociate-project-assets-errors-schema.json\",\n  \"title\": \"BatchDisassociateProjectAssetsErrors\",\n  \"description\": \"BatchDisassociateProjectAssetsErrors schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"assetId\",\n      \"code\",\n      \"message\"\n    ],\n    \"properties\": {\n      \"assetId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \"The ID of the asset.\"\n          }\n        ]\n      },\n      \"code\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AssetErrorCode\"\n          },\n          {\n            \"description\": \"The error code.\"\n          }\n       \
  \ ]\n      },\n      \"message\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AssetErrorMessage\"\n          },\n          {\n            \"description\": \"The error message.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains error details for the requested associate project asset action.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-disassociate-project-assets-errors-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchDisassociateProjectAssetsErrors
---
