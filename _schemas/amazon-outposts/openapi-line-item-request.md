---
description: Information about a line item request.
layout: schema
name: LineItemRequest
properties_list:
- description: ''
  name: CatalogItemId
  type: object
- description: ''
  name: Quantity
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-line-item-request-schema.json
slug: openapi-line-item-request
source_filename: openapi-line-item-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-line-item-request-schema.json\",\n  \"title\": \"LineItemRequest\",\n  \"description\": \"Information about a line item request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogItemId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SkuCode\"\n        },\n        {\n          \"description\": \"The ID of the catalog item.\"\n        }\n      ]\n    },\n    \"Quantity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LineItemQuantity\"\n        },\n        {\n          \"description\": \"The quantity of a line item request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-line-item-request-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: LineItemRequest
---
