---
description: Contains a summary of an associated asset.
layout: schema
name: AssociatedAssetsSummary
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: assetModelId
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: lastUpdateDate
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: hierarchies
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-associated-assets-summary-schema.json
slug: iot-sitewise-associated-assets-summary
source_filename: iot-sitewise-associated-assets-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-associated-assets-summary-schema.json\",\n  \"title\": \"AssociatedAssetsSummary\",\n  \"description\": \"Contains a summary of an associated asset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the asset.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the asset, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:asset/${AssetId}</code> </p>\"\n\
  \        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the asset.\"\n        }\n      ]\n    },\n    \"assetModelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the asset model used to create the asset.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the asset was created, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"lastUpdateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the asset was last updated, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"status\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetStatus\"\n        },\n        {\n          \"description\": \"The current status of the asset.\"\n        }\n      ]\n    },\n    \"hierarchies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetHierarchies\"\n        },\n        {\n          \"description\": \"A list of asset hierarchies that each contain a <code>hierarchyId</code>. A hierarchy specifies allowed parent/child asset relationships.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description for the asset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"arn\",\n    \"name\",\n    \"assetModelId\",\n    \"creationDate\",\n    \"lastUpdateDate\",\n    \"status\",\n    \"hierarchies\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-associated-assets-summary-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssociatedAssetsSummary
---
