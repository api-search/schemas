---
description: Library analytics action data broken down by team.
layout: schema
name: LibraryAnalyticsActionsByTeam
properties_list:
- description: The date in ISO 8601 format. e.g. 2023-12-13
  name: week
  type: string
- description: The name of the team using the library.
  name: teamName
  type: string
- description: The name of the workspace that the team belongs to.
  name: workspaceName
  type: string
- description: The number of detach events for this period.
  name: detachments
  type: number
- description: The number of insertion events for this period.
  name: insertions
  type: number
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-analytics-library-analytics-actions-by-team-schema.json
slug: figma-analytics-library-analytics-actions-by-team
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LibraryAnalyticsActionsByTeam\",\n  \"type\": \"object\",\n  \"description\": \"Library analytics action data broken down by team.\",\n  \"properties\": {\n    \"week\": {\n      \"type\": \"string\",\n      \"description\": \"The date in ISO 8601 format. e.g. 2023-12-13\"\n    },\n    \"teamName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the team using the library.\"\n    },\n    \"workspaceName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workspace that the team belongs to.\"\n    },\n    \"detachments\": {\n      \"type\": \"number\",\n      \"description\": \"The number of detach events for this period.\"\n    },\n    \"insertions\": {\n      \"type\": \"number\",\n      \"description\": \"The number of insertion events for this period.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-analytics-library-analytics-actions-by-team-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: LibraryAnalyticsActionsByTeam
---
