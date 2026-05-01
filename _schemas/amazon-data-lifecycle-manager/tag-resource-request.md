---
description: Request body for adding tags to a resource.
layout: schema
name: Tag Resource Request
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon Data Lifecycle Manager
provider_slug: amazon-data-lifecycle-manager
schema_file: json-schema/tag-resource-request-schema.json
slug: tag-resource-request
source_filename: tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-lifecycle-manager/json-schema/tag-resource-request-schema.json\",\n  \"title\": \"Tag Resource Request\",\n  \"description\": \"Request body for adding tags to a resource.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Tags\"\n  ],\n  \"properties\": {\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-lifecycle-manager/refs/heads/main/json-schema/tag-resource-request-schema.json
tags:
- Backup
- EBS Snapshots
- Lifecycle Management
- Storage
- Automation
- Compliance
title: Tag Resource Request
---
