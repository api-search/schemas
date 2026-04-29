---
description: ListCatalogItemsOutput schema from Amazon Outposts
layout: schema
name: ListCatalogItemsOutput
properties_list:
- description: ''
  name: CatalogItems
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-list-catalog-items-output-schema.json
slug: openapi-list-catalog-items-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-list-catalog-items-output-schema.json\",\n  \"title\": \"ListCatalogItemsOutput\",\n  \"description\": \"ListCatalogItemsOutput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogItems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogItemListDefinition\"\n        },\n        {\n          \"description\": \"Information about the catalog items.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/Token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-list-catalog-items-output-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: ListCatalogItemsOutput
---
