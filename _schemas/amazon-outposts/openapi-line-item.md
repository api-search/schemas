---
description: Information about a line item.
layout: schema
name: LineItem
properties_list:
- description: ''
  name: CatalogItemId
  type: object
- description: ''
  name: LineItemId
  type: object
- description: ''
  name: Quantity
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: ShipmentInformation
  type: object
- description: ''
  name: AssetInformationList
  type: object
- description: ''
  name: PreviousLineItemId
  type: object
- description: ''
  name: PreviousOrderId
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-line-item-schema.json
slug: openapi-line-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-line-item-schema.json\",\n  \"title\": \"LineItem\",\n  \"description\": \"Information about a line item.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogItemId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SkuCode\"\n        },\n        {\n          \"description\": \" The ID of the catalog item. \"\n        }\n      ]\n    },\n    \"LineItemId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LineItemId\"\n        },\n        {\n          \"description\": \"The ID of the line item.\"\n        }\n      ]\n    },\n    \"Quantity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LineItemQuantity\"\n        },\n        {\n          \"description\": \"The quantity of the line item.\"\n    \
  \    }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LineItemStatus\"\n        },\n        {\n          \"description\": \"The status of the line item.\"\n        }\n      ]\n    },\n    \"ShipmentInformation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShipmentInformation\"\n        },\n        {\n          \"description\": \" Information about a line item shipment. \"\n        }\n      ]\n    },\n    \"AssetInformationList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LineItemAssetInformationList\"\n        },\n        {\n          \"description\": \" Information about assets. \"\n        }\n      ]\n    },\n    \"PreviousLineItemId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LineItemId\"\n        },\n        {\n          \"description\": \"The ID of the previous line item.\"\n        }\n      ]\n    },\n    \"PreviousOrderId\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderId\"\n        },\n        {\n          \"description\": \"The ID of the previous order.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-line-item-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: LineItem
---
