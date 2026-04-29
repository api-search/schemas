---
description: <p>The routing configuration for a fleet alias.</p> <p> <b>Related actions</b> </p> <p> <a href="https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets">All APIs by task</a> </p>
layout: schema
name: RoutingStrategy
properties_list:
- description: ''
  name: Type
  type: object
- description: ''
  name: FleetId
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-routing-strategy-schema.json
slug: gamelift-routing-strategy
source_filename: gamelift-routing-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-routing-strategy-schema.json\",\n  \"title\": \"RoutingStrategy\",\n  \"description\": \"<p>The routing configuration for a fleet alias.</p> <p> <b>Related actions</b> </p> <p> <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets\\\">All APIs by task</a> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoutingStrategyType\"\n        },\n        {\n          \"description\": \"<p>The type of routing strategy for the alias.</p> <p>Possible routing types include the following:</p> <ul> <li> <p> <b>SIMPLE</b> - The alias resolves to one specific fleet. Use this type when routing to active fleets.</p> </li> <li> <p> <b>TERMINAL</b>\
  \ - The alias does not resolve to a fleet but instead can be used to display a message to the user. A terminal alias throws a TerminalRoutingStrategyException with the message embedded.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetId\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet that the alias points to. This value is the fleet ID, not the fleet ARN.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FreeText\"\n        },\n        {\n          \"description\": \"The message text to be used with a terminal routing strategy.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-routing-strategy-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: RoutingStrategy
---
