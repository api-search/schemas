---
description: Runtime configuration for APPSYNC_JS resolvers
layout: schema
name: AppSyncRuntime
properties_list:
- description: Runtime name
  name: name
  type: string
- description: Runtime version
  name: runtimeVersion
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-app-sync-runtime-schema.json
slug: appsync-app-sync-runtime
source_filename: appsync-app-sync-runtime-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-app-sync-runtime-schema.json\",\n  \"title\": \"AppSyncRuntime\",\n  \"description\": \"Runtime configuration for APPSYNC_JS resolvers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Runtime name\"\n    },\n    \"runtimeVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Runtime version\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-app-sync-runtime-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: AppSyncRuntime
---
