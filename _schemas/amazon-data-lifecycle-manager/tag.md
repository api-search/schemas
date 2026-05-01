---
description: A key-value tag pair applied to an AWS resource.
layout: schema
name: Tag
properties_list:
- description: The tag key
  name: Key
  type: string
- description: The tag value
  name: Value
  type: string
provider_name: Amazon Data Lifecycle Manager
provider_slug: amazon-data-lifecycle-manager
schema_file: json-schema/tag-schema.json
slug: tag
source_filename: tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-lifecycle-manager/json-schema/tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A key-value tag pair applied to an AWS resource.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ],\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"The tag key\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"The tag value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-lifecycle-manager/refs/heads/main/json-schema/tag-schema.json
tags:
- Backup
- EBS Snapshots
- Lifecycle Management
- Storage
- Automation
- Compliance
title: Tag
---
