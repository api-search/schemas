---
description: ''
layout: schema
name: CardMoveRequest
properties_list:
- description: Recording ID of the card to move
  name: source_id
  type: integer
- description: Recording ID of the destination column
  name: target_id
  type: integer
- description: Zero-indexed position within the destination column
  name: position
  type: integer
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/cardmoverequest-schema.json
slug: cardmoverequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/cardmoverequest-schema.json\",\n  \"title\": \"CardMoveRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"source_id\",\n    \"target_id\",\n    \"position\"\n  ],\n  \"properties\": {\n    \"source_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Recording ID of the card to move\"\n    },\n    \"target_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Recording ID of the destination column\"\n    },\n    \"position\": {\n      \"type\": \"integer\",\n      \"description\": \"Zero-indexed position within the destination column\",\n      \"minimum\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/cardmoverequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: CardMoveRequest
---
