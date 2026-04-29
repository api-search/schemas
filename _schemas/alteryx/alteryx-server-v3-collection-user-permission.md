---
description: User permissions within a collection
layout: schema
name: CollectionUserPermission
properties_list:
- description: ID of the user
  name: userId
  type: string
- description: ''
  name: isAdmin
  type: boolean
- description: ''
  name: canAddAssets
  type: boolean
- description: ''
  name: canRemoveAssets
  type: boolean
- description: ''
  name: canUpdateAssets
  type: boolean
- description: ''
  name: canAddUsers
  type: boolean
- description: ''
  name: canRemoveUsers
  type: boolean
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-collection-user-permission-schema.json
slug: alteryx-server-v3-collection-user-permission
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CollectionUserPermission\",\n  \"type\": \"object\",\n  \"description\": \"User permissions within a collection\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user\"\n    },\n    \"isAdmin\": {\n      \"type\": \"boolean\"\n    },\n    \"canAddAssets\": {\n      \"type\": \"boolean\"\n    },\n    \"canRemoveAssets\": {\n      \"type\": \"boolean\"\n    },\n    \"canUpdateAssets\": {\n      \"type\": \"boolean\"\n    },\n    \"canAddUsers\": {\n      \"type\": \"boolean\"\n    },\n    \"canRemoveUsers\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-collection-user-permission-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: CollectionUserPermission
---
