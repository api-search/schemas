---
description: Request body for creating a new revision.
layout: schema
name: Create Revision Request
properties_list:
- description: ''
  name: Comment
  type: string
- description: ''
  name: Tags
  type: object
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/create-revision-request-schema.json
slug: create-revision-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/create-revision-request-schema.json\",\n  \"title\": \"Create Revision Request\",\n  \"description\": \"Request body for creating a new revision.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Comment\": {\n      \"type\": \"string\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/create-revision-request-schema.json
tags:
- AWS
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: Create Revision Request
---
