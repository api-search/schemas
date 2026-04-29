---
description: Represents an identity of an actor
layout: schema
name: Identity
properties_list:
- description: The display name of the identity
  name: displayName
  type: string
- description: The unique identifier of the identity
  name: id
  type: string
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-identity-schema.json
slug: microsoft-planner-identity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Identity\",\n  \"type\": \"object\",\n  \"description\": \"Represents an identity of an actor\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the identity\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the identity\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-identity-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: Identity
---
