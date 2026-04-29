---
description: Specifies an inventory filter. The inventory only includes objects that meet the filter's criteria.
layout: schema
name: InventoryFilter
properties_list:
- description: ''
  name: Prefix
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-inventoryfilter-schema.json
slug: s3-inventoryfilter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InventoryFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefix\": {}\n  },\n  \"required\": [\n    \"Prefix\"\n  ],\n  \"description\": \"Specifies an inventory filter. The inventory only includes objects that meet the filter's criteria.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-inventoryfilter-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: InventoryFilter
---
