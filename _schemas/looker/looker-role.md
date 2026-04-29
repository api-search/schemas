---
description: A role defines a set of permissions and model access controls that can be assigned to users and groups.
layout: schema
name: Role
properties_list:
- description: Unique numeric identifier
  name: id
  type: integer
- description: Display name of the role
  name: name
  type: string
- description: ID of the permission set assigned to this role
  name: permission_set_id
  type: integer
- description: ID of the model set assigned to this role
  name: model_set_id
  type: integer
- description: Number of users with this role
  name: user_count
  type: integer
- description: Relative URL for this role
  name: url
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-role-schema.json
slug: looker-role
source_filename: looker-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Role\",\n  \"type\": \"object\",\n  \"description\": \"A role defines a set of permissions and model access controls that can be assigned to users and groups.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the role\"\n    },\n    \"permission_set_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the permission set assigned to this role\"\n    },\n    \"model_set_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the model set assigned to this role\"\n    },\n    \"user_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of users with this role\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URL for this role\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-role-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: Role
---
