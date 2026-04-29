---
description: DescribeAssetModelResponse schema
layout: schema
name: DescribeAssetModelResponse
properties_list:
- description: ''
  name: assetModelId
  type: object
- description: ''
  name: assetModelArn
  type: object
- description: ''
  name: assetModelName
  type: object
- description: ''
  name: assetModelDescription
  type: object
- description: ''
  name: assetModelProperties
  type: object
- description: ''
  name: assetModelHierarchies
  type: object
- description: ''
  name: assetModelCompositeModels
  type: object
- description: ''
  name: assetModelCreationDate
  type: object
- description: ''
  name: assetModelLastUpdateDate
  type: object
- description: ''
  name: assetModelStatus
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-describe-asset-model-response-schema.json
slug: iot-sitewise-describe-asset-model-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-asset-model-response-schema.json\",\n  \"title\": \"DescribeAssetModelResponse\",\n  \"description\": \"DescribeAssetModelResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetModelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the asset model.\"\n        }\n      ]\n    },\n    \"assetModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the asset model, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:asset-model/${AssetModelId}</code>\
  \ </p>\"\n        }\n      ]\n    },\n    \"assetModelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the asset model.\"\n        }\n      ]\n    },\n    \"assetModelDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The asset model's description.\"\n        }\n      ]\n    },\n    \"assetModelProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetModelProperties\"\n        },\n        {\n          \"description\": \"<p>The list of asset properties for the asset model.</p> <p>This object doesn't include properties that you define in composite models. You can find composite model properties in the <code>assetModelCompositeModels</code> object.</p>\"\n        }\n      ]\n    },\n    \"assetModelHierarchies\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/AssetModelHierarchies\"\n        },\n        {\n          \"description\": \"A list of asset model hierarchies that each contain a <code>childAssetModelId</code> and a <code>hierarchyId</code> (named <code>id</code>). A hierarchy specifies allowed parent/child asset relationships for an asset model.\"\n        }\n      ]\n    },\n    \"assetModelCompositeModels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetModelCompositeModels\"\n        },\n        {\n          \"description\": \"The list of composite asset models for the asset model.\"\n        }\n      ]\n    },\n    \"assetModelCreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the asset model was created, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"assetModelLastUpdateDate\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the asset model was last updated, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"assetModelStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetModelStatus\"\n        },\n        {\n          \"description\": \"The current status of the asset model, which contains a state and any error message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"assetModelId\",\n    \"assetModelArn\",\n    \"assetModelName\",\n    \"assetModelDescription\",\n    \"assetModelProperties\",\n    \"assetModelHierarchies\",\n    \"assetModelCreationDate\",\n    \"assetModelLastUpdateDate\",\n    \"assetModelStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-asset-model-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DescribeAssetModelResponse
---
