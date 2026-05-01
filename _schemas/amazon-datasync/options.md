---
description: Configuration options for a DataSync task defining transfer behavior.
layout: schema
name: Options
properties_list:
- description: ''
  name: VerifyMode
  type: string
- description: ''
  name: OverwriteMode
  type: string
- description: ''
  name: Atime
  type: string
- description: ''
  name: Mtime
  type: string
- description: ''
  name: PreserveDeletedFiles
  type: string
provider_name: Amazon DataSync
provider_slug: amazon-datasync
schema_file: json-schema/options-schema.json
slug: options
source_filename: options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datasync/json-schema/options-schema.json\",\n  \"title\": \"Options\",\n  \"description\": \"Configuration options for a DataSync task defining transfer behavior.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VerifyMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POINT_IN_TIME_CONSISTENT\",\n        \"ONLY_FILES_TRANSFERRED\",\n        \"NONE\"\n      ]\n    },\n    \"OverwriteMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ALWAYS\",\n        \"NEVER\"\n      ]\n    },\n    \"Atime\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NONE\",\n        \"BEST_EFFORT\"\n      ]\n    },\n    \"Mtime\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NONE\",\n        \"PRESERVE\"\n      ]\n    },\n    \"PreserveDeletedFiles\": {\n      \"type\": \"string\",\n      \"enum\": [\n       \
  \ \"PRESERVE\",\n        \"REMOVE\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/json-schema/options-schema.json
tags:
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
title: Options
---
