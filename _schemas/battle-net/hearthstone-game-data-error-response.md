---
description: An error response from the API.
layout: schema
name: ErrorResponse
properties_list:
- description: HTTP error code.
  name: code
  type: integer
- description: Error type.
  name: type
  type: string
- description: A description of the error.
  name: detail
  type: string
provider_name: Battle.net
provider_slug: battle-net
schema_file: json-schema/hearthstone-game-data-error-response-schema.json
slug: hearthstone-game-data-error-response
source_filename: hearthstone-game-data-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"An error response from the API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP error code.\",\n      \"example\": 404\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Error type.\",\n      \"example\": \"BLZWEBAPI00000404\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the error.\",\n      \"example\": \"Not Found\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-error-response-schema.json
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: ErrorResponse
---
