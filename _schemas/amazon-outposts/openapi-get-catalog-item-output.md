---
description: GetCatalogItemOutput schema from Amazon Outposts
layout: schema
name: GetCatalogItemOutput
properties_list:
- description: ''
  name: CatalogItem
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-get-catalog-item-output-schema.json
slug: openapi-get-catalog-item-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-get-catalog-item-output-schema.json\",\n  \"title\": \"GetCatalogItemOutput\",\n  \"description\": \"GetCatalogItemOutput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogItem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogItem\"\n        },\n        {\n          \"description\": \"Information about this catalog item.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-get-catalog-item-output-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: GetCatalogItemOutput
---
