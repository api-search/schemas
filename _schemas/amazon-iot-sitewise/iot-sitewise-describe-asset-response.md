---
description: DescribeAssetResponse schema
layout: schema
name: DescribeAssetResponse
properties_list:
- description: ''
  name: assetId
  type: object
- description: ''
  name: assetArn
  type: object
- description: ''
  name: assetName
  type: object
- description: ''
  name: assetModelId
  type: object
- description: ''
  name: assetProperties
  type: object
- description: ''
  name: assetHierarchies
  type: object
- description: ''
  name: assetCompositeModels
  type: object
- description: ''
  name: assetCreationDate
  type: object
- description: ''
  name: assetLastUpdateDate
  type: object
- description: ''
  name: assetStatus
  type: object
- description: ''
  name: assetDescription
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-describe-asset-response-schema.json
slug: iot-sitewise-describe-asset-response
source_filename: iot-sitewise-describe-asset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-asset-response-schema.json\",\n  \"title\": \"DescribeAssetResponse\",\n  \"description\": \"DescribeAssetResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the asset.\"\n        }\n      ]\n    },\n    \"assetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the asset, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:asset/${AssetId}</code> </p>\"\n        }\n\
  \      ]\n    },\n    \"assetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the asset.\"\n        }\n      ]\n    },\n    \"assetModelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the asset model that was used to create the asset.\"\n        }\n      ]\n    },\n    \"assetProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetProperties\"\n        },\n        {\n          \"description\": \"<p>The list of asset properties for the asset.</p> <p>This object doesn't include properties that you define in composite models. You can find composite model properties in the <code>assetCompositeModels</code> object.</p>\"\n        }\n      ]\n    },\n    \"assetHierarchies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetHierarchies\"\
  \n        },\n        {\n          \"description\": \"A list of asset hierarchies that each contain a <code>hierarchyId</code>. A hierarchy specifies allowed parent/child asset relationships.\"\n        }\n      ]\n    },\n    \"assetCompositeModels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetCompositeModels\"\n        },\n        {\n          \"description\": \"The composite models for the asset.\"\n        }\n      ]\n    },\n    \"assetCreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the asset was created, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"assetLastUpdateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the asset was last updated, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"assetStatus\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetStatus\"\n        },\n        {\n          \"description\": \"The current status of the asset, which contains a state and any error message.\"\n        }\n      ]\n    },\n    \"assetDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description for the asset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"assetId\",\n    \"assetArn\",\n    \"assetName\",\n    \"assetModelId\",\n    \"assetProperties\",\n    \"assetHierarchies\",\n    \"assetCreationDate\",\n    \"assetLastUpdateDate\",\n    \"assetStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-asset-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DescribeAssetResponse
---
