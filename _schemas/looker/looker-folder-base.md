---
description: Basic folder information
layout: schema
name: FolderBase
properties_list:
- description: Unique identifier
  name: id
  type: string
- description: Display name
  name: name
  type: string
- description: Parent folder ID
  name: parent_id
  type: string
- description: Content metadata ID
  name: content_metadata_id
  type: integer
- description: Whether this is the shared root folder
  name: is_shared_root
  type: boolean
- description: Whether this is the users root folder
  name: is_users_root
  type: boolean
- description: Whether this is a user's personal root folder
  name: is_user_root
  type: boolean
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-folder-base-schema.json
slug: looker-folder-base
source_filename: looker-folder-base-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FolderBase\",\n  \"type\": \"object\",\n  \"description\": \"Basic folder information\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name\"\n    },\n    \"parent_id\": {\n      \"type\": \"string\",\n      \"description\": \"Parent folder ID\"\n    },\n    \"content_metadata_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Content metadata ID\"\n    },\n    \"is_shared_root\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the shared root folder\"\n    },\n    \"is_users_root\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the users root folder\"\n    },\n    \"is_user_root\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a user's personal root\
  \ folder\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-folder-base-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: FolderBase
---
