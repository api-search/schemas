---
description: Request body for adding tags to a resource.
layout: schema
name: Tag Resource Request
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/tag-resource-request-schema.json
slug: tag-resource-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/tag-resource-request-schema.json\",\n  \"title\": \"Tag Resource Request\",\n  \"description\": \"Request body for adding tags to a resource.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Tags\"\n  ],\n  \"properties\": {\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/tag-resource-request-schema.json
tags:
- AWS
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: Tag Resource Request
---
