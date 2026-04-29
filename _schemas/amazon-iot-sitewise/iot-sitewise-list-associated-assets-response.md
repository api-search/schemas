---
description: ListAssociatedAssetsResponse schema
layout: schema
name: ListAssociatedAssetsResponse
properties_list:
- description: ''
  name: assetSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-list-associated-assets-response-schema.json
slug: iot-sitewise-list-associated-assets-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-associated-assets-response-schema.json\",\n  \"title\": \"ListAssociatedAssetsResponse\",\n  \"description\": \"ListAssociatedAssetsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssociatedAssetsSummaries\"\n        },\n        {\n          \"description\": \"A list that summarizes the associated assets.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"assetSummaries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-associated-assets-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: ListAssociatedAssetsResponse
---
