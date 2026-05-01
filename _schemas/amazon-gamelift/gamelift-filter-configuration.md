---
description: A list of fleet locations where a game session queue can place new game sessions. You can use a filter to temporarily turn off placements for specific locations. For queues that have multi-location fleets, you can use a filter configuration allow placement with some, but not all of these locations.
layout: schema
name: FilterConfiguration
properties_list:
- description: ''
  name: AllowedLocations
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-filter-configuration-schema.json
slug: gamelift-filter-configuration
source_filename: gamelift-filter-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-filter-configuration-schema.json\",\n  \"title\": \"FilterConfiguration\",\n  \"description\": \"A list of fleet locations where a game session queue can place new game sessions. You can use a filter to temporarily turn off placements for specific locations. For queues that have multi-location fleets, you can use a filter configuration allow placement with some, but not all of these locations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AllowedLocations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationList\"\n        },\n        {\n          \"description\": \" A list of locations to allow game session placement in, in the form of Amazon Web Services Region codes such as <code>us-west-2</code>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-filter-configuration-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: FilterConfiguration
---
