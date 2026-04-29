---
description: A user in a Power BI workspace
layout: schema
name: GroupUser
properties_list:
- description: The email address of the user
  name: emailAddress
  type: string
- description: The display name of the user
  name: displayName
  type: string
- description: The object ID of the user
  name: identifier
  type: string
- description: The Microsoft Graph ID of the user
  name: graphId
  type: string
- description: The access right of the user in the workspace
  name: groupUserAccessRight
  type: string
- description: The principal type
  name: principalType
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-group-user-schema.json
slug: power-bi-rest-group-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupUser\",\n  \"type\": \"object\",\n  \"description\": \"A user in a Power BI workspace\",\n  \"properties\": {\n    \"emailAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the user\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the user\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the user\"\n    },\n    \"graphId\": {\n      \"type\": \"string\",\n      \"description\": \"The Microsoft Graph ID of the user\"\n    },\n    \"groupUserAccessRight\": {\n      \"type\": \"string\",\n      \"description\": \"The access right of the user in the workspace\"\n    },\n    \"principalType\": {\n      \"type\": \"string\",\n      \"description\": \"The principal type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-group-user-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: GroupUser
---
