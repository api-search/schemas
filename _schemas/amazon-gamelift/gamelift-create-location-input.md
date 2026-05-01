---
description: CreateLocationInput schema from Amazon GameLift API
layout: schema
name: CreateLocationInput
properties_list:
- description: ''
  name: LocationName
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-location-input-schema.json
slug: gamelift-create-location-input
source_filename: gamelift-create-location-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-location-input-schema.json\",\n  \"title\": \"CreateLocationInput\",\n  \"description\": \"CreateLocationInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LocationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomInputLocationStringModel\"\n        },\n        {\n          \"description\": \"A descriptive name for the custom location.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A list of labels to assign to the new matchmaking configuration resource. Tags are developer-defined key-value pairs. Tagging Amazon Web Services resources are useful for resource management,\
  \ access management and cost allocation. For more information, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\"> Tagging Amazon Web Services Resources</a> in the <i>Amazon Web Services General Rareference</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LocationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-location-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateLocationInput
---
