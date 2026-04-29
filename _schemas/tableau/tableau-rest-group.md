---
description: ''
layout: schema
name: Group
properties_list:
- description: The unique identifier for the group.
  name: id
  type: string
- description: The name of the group.
  name: name
  type: string
- description: The domain name for Active Directory groups. For local groups, this is "local".
  name: domainName
  type: string
- description: The minimum site role for members of the group when they are imported from Active Directory.
  name: minimumSiteRole
  type: string
- description: The number of users in the group.
  name: userCount
  type: integer
- description: ''
  name: import
  type: object
provider_name: Tableau
provider_slug: tableau
schema_file: json-schema/tableau-rest-group-schema.json
slug: tableau-rest-group
source_filename: tableau-rest-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the group.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the group.\"\n    },\n    \"domainName\": {\n      \"type\": \"string\",\n      \"description\": \"The domain name for Active Directory groups. For local groups, this is \\\"local\\\".\"\n    },\n    \"minimumSiteRole\": {\n      \"type\": \"string\",\n      \"description\": \"The minimum site role for members of the group when they are imported from Active Directory.\"\n    },\n    \"userCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of users in the group.\"\n    },\n    \"import\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/json-schema/tableau-rest-group-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
title: Group
---
