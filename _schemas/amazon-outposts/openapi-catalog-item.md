---
description: Information about a catalog item.
layout: schema
name: CatalogItem
properties_list:
- description: ''
  name: CatalogItemId
  type: object
- description: ''
  name: ItemStatus
  type: object
- description: ''
  name: EC2Capacities
  type: object
- description: ''
  name: PowerKva
  type: object
- description: ''
  name: WeightLbs
  type: object
- description: ''
  name: SupportedUplinkGbps
  type: object
- description: ''
  name: SupportedStorage
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-catalog-item-schema.json
slug: openapi-catalog-item
source_filename: openapi-catalog-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-catalog-item-schema.json\",\n  \"title\": \"CatalogItem\",\n  \"description\": \" Information about a catalog item. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogItemId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SkuCode\"\n        },\n        {\n          \"description\": \" The ID of the catalog item. \"\n        }\n      ]\n    },\n    \"ItemStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogItemStatus\"\n        },\n        {\n          \"description\": \" The status of a catalog item. \"\n        }\n      ]\n    },\n    \"EC2Capacities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2CapacityListDefinition\"\n        },\n        {\n          \"description\": \"\
  \ Information about the EC2 capacity of an item. \"\n        }\n      ]\n    },\n    \"PowerKva\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogItemPowerKva\"\n        },\n        {\n          \"description\": \" Information about the power draw of an item. \"\n        }\n      ]\n    },\n    \"WeightLbs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogItemWeightLbs\"\n        },\n        {\n          \"description\": \" The weight of the item in pounds. \"\n        }\n      ]\n    },\n    \"SupportedUplinkGbps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SupportedUplinkGbpsListDefinition\"\n        },\n        {\n          \"description\": \" The uplink speed this catalog item requires for the connection to the Region. \"\n        }\n      ]\n    },\n    \"SupportedStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SupportedStorageList\"\n\
  \        },\n        {\n          \"description\": \" The supported storage options for the catalog item. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-catalog-item-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: CatalogItem
---
