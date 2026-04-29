---
description: CreateAssetModelResponse schema
layout: schema
name: CreateAssetModelResponse
properties_list:
- description: ''
  name: assetModelId
  type: object
- description: ''
  name: assetModelArn
  type: object
- description: ''
  name: assetModelStatus
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-create-asset-model-response-schema.json
slug: iot-sitewise-create-asset-model-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-asset-model-response-schema.json\",\n  \"title\": \"CreateAssetModelResponse\",\n  \"description\": \"CreateAssetModelResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetModelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the asset model. You can use this ID when you call other IoT SiteWise APIs.\"\n        }\n      ]\n    },\n    \"assetModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the asset model, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:asset-model/${AssetModelId}</code>\
  \ </p>\"\n        }\n      ]\n    },\n    \"assetModelStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetModelStatus\"\n        },\n        {\n          \"description\": \"The status of the asset model, which contains a state (<code>CREATING</code> after successfully calling this operation) and any error message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"assetModelId\",\n    \"assetModelArn\",\n    \"assetModelStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-asset-model-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: CreateAssetModelResponse
---
