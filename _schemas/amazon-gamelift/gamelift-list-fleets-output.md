---
description: ListFleetsOutput schema from Amazon GameLift API
layout: schema
name: ListFleetsOutput
properties_list:
- description: ''
  name: FleetIds
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-list-fleets-output-schema.json
slug: gamelift-list-fleets-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-list-fleets-output-schema.json\",\n  \"title\": \"ListFleetsOutput\",\n  \"description\": \"ListFleetsOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdList\"\n        },\n        {\n          \"description\": \"A set of fleet IDs that match the list request.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates where to resume retrieving results on the next call to this operation. If no token is returned, these results represent the end of the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-list-fleets-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ListFleetsOutput
---
