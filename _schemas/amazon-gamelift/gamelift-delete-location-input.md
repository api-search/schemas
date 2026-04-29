---
description: DeleteLocationInput schema from Amazon GameLift API
layout: schema
name: DeleteLocationInput
properties_list:
- description: ''
  name: LocationName
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-delete-location-input-schema.json
slug: gamelift-delete-location-input
source_filename: gamelift-delete-location-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-location-input-schema.json\",\n  \"title\": \"DeleteLocationInput\",\n  \"description\": \"DeleteLocationInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LocationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomLocationNameOrArnModel\"\n        },\n        {\n          \"description\": \"The location name of the custom location to be deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LocationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-location-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DeleteLocationInput
---
