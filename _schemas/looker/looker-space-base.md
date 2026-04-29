---
description: Basic space (folder) information
layout: schema
name: SpaceBase
properties_list:
- description: Unique identifier
  name: id
  type: string
- description: Display name
  name: name
  type: string
- description: Parent space ID
  name: parent_id
  type: string
- description: Whether this is the shared root space
  name: is_shared_root
  type: boolean
- description: Whether this is the users root space
  name: is_users_root
  type: boolean
- description: Whether this is a user's personal root space
  name: is_user_root
  type: boolean
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-space-base-schema.json
slug: looker-space-base
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SpaceBase\",\n  \"type\": \"object\",\n  \"description\": \"Basic space (folder) information\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name\"\n    },\n    \"parent_id\": {\n      \"type\": \"string\",\n      \"description\": \"Parent space ID\"\n    },\n    \"is_shared_root\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the shared root space\"\n    },\n    \"is_users_root\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the users root space\"\n    },\n    \"is_user_root\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a user's personal root space\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-space-base-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: SpaceBase
---
