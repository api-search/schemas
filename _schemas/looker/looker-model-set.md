---
description: A set of LookML models that can be assigned to a role
layout: schema
name: ModelSet
properties_list:
- description: Unique numeric identifier
  name: id
  type: integer
- description: Display name
  name: name
  type: string
- description: List of model names included in this set
  name: models
  type: array
- description: Whether this is a built-in model set
  name: built_in
  type: boolean
- description: Whether this grants access to all models
  name: all_access
  type: boolean
- description: Relative URL
  name: url
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-model-set-schema.json
slug: looker-model-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModelSet\",\n  \"type\": \"object\",\n  \"description\": \"A set of LookML models that can be assigned to a role\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name\"\n    },\n    \"models\": {\n      \"type\": \"array\",\n      \"description\": \"List of model names included in this set\"\n    },\n    \"built_in\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a built-in model set\"\n    },\n    \"all_access\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this grants access to all models\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-model-set-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: ModelSet
---
