---
description: Amazon GameLift Anywhere configuration options for your Anywhere fleets.
layout: schema
name: AnywhereConfiguration
properties_list:
- description: ''
  name: Cost
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-anywhere-configuration-schema.json
slug: gamelift-anywhere-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-anywhere-configuration-schema.json\",\n  \"title\": \"AnywhereConfiguration\",\n  \"description\": \"Amazon GameLift Anywhere configuration options for your Anywhere fleets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Cost\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonNegativeLimitedLengthDouble\"\n        },\n        {\n          \"description\": \"The cost to run your fleet per hour. Amazon GameLift uses the provided cost of your fleet to balance usage in queues. For more information about queues, see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/queues-intro.html\\\">Setting up queues</a> in the <i>Amazon GameLift Developer Guide</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Cost\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-anywhere-configuration-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: AnywhereConfiguration
---
