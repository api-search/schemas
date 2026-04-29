---
description: ListTagsForResourceRequest schema from Amazon Marketplace API
layout: schema
name: ListTagsForResourceRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-list-tags-for-resource-request-schema.json
slug: amazon-marketplace-list-tags-for-resource-request
source_filename: amazon-marketplace-list-tags-for-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-list-tags-for-resource-request-schema.json\",\n  \"title\": \"ListTagsForResourceRequest\",\n  \"description\": \"ListTagsForResourceRequest schema from Amazon Marketplace API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"Required. The Amazon Resource Name (ARN) associated with the resource you want to list tags on.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-list-tags-for-resource-request-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: ListTagsForResourceRequest
---
