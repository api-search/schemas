---
description: An asset owned by a user
layout: schema
name: UserAsset
properties_list:
- description: Asset identifier
  name: id
  type: string
- description: Type of asset (workflow, schedule, collection)
  name: type
  type: string
- description: Name of the asset
  name: name
  type: string
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-user-asset-schema.json
slug: alteryx-server-v3-user-asset
source_filename: alteryx-server-v3-user-asset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserAsset\",\n  \"type\": \"object\",\n  \"description\": \"An asset owned by a user\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Asset identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of asset (workflow, schedule, collection)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the asset\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-user-asset-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: UserAsset
---
