---
description: Sync configuration for conflict resolution
layout: schema
name: SyncConfig
properties_list:
- description: Conflict handler type
  name: conflictHandler
  type: string
- description: Conflict detection type
  name: conflictDetection
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-sync-config-schema.json
slug: appsync-sync-config
source_filename: appsync-sync-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-sync-config-schema.json\",\n  \"title\": \"SyncConfig\",\n  \"description\": \"Sync configuration for conflict resolution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"conflictHandler\": {\n      \"type\": \"string\",\n      \"description\": \"Conflict handler type\"\n    },\n    \"conflictDetection\": {\n      \"type\": \"string\",\n      \"description\": \"Conflict detection type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-sync-config-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: SyncConfig
---
