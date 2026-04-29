---
description: CreateAssetResponse schema
layout: schema
name: CreateAssetResponse
properties_list:
- description: ''
  name: assetId
  type: object
- description: ''
  name: assetArn
  type: object
- description: ''
  name: assetStatus
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-create-asset-response-schema.json
slug: iot-sitewise-create-asset-response
source_filename: iot-sitewise-create-asset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-asset-response-schema.json\",\n  \"title\": \"CreateAssetResponse\",\n  \"description\": \"CreateAssetResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the asset. This ID uniquely identifies the asset within IoT SiteWise and can be used with other IoT SiteWise APIs.\"\n        }\n      ]\n    },\n    \"assetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the asset, which has the following format.</p> <p>\
  \ <code>arn:${Partition}:iotsitewise:${Region}:${Account}:asset/${AssetId}</code> </p>\"\n        }\n      ]\n    },\n    \"assetStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetStatus\"\n        },\n        {\n          \"description\": \"The status of the asset, which contains a state (<code>CREATING</code> after successfully calling this operation) and any error message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"assetId\",\n    \"assetArn\",\n    \"assetStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-asset-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: CreateAssetResponse
---
