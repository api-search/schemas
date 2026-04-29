---
description: Response from the Get Team Projects endpoint.
layout: schema
name: GetTeamProjectsResponse
properties_list:
- description: The name of the team.
  name: name
  type: string
- description: ''
  name: projects
  type: array
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-get-team-projects-response-schema.json
slug: figma-rest-get-team-projects-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetTeamProjectsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response from the Get Team Projects endpoint.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the team.\"\n    },\n    \"projects\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-get-team-projects-response-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: GetTeamProjectsResponse
---
