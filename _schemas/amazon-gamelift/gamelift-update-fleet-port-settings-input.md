---
description: UpdateFleetPortSettingsInput schema from Amazon GameLift API
layout: schema
name: UpdateFleetPortSettingsInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: InboundPermissionAuthorizations
  type: object
- description: ''
  name: InboundPermissionRevocations
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-fleet-port-settings-input-schema.json
slug: gamelift-update-fleet-port-settings-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-fleet-port-settings-input-schema.json\",\n  \"title\": \"UpdateFleetPortSettingsInput\",\n  \"description\": \"UpdateFleetPortSettingsInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to update port settings for. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    },\n    \"InboundPermissionAuthorizations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpPermissionsList\"\n        },\n        {\n          \"description\": \"A collection of port settings to be added to the fleet resource.\"\n        }\n  \
  \    ]\n    },\n    \"InboundPermissionRevocations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpPermissionsList\"\n        },\n        {\n          \"description\": \"A collection of port settings to be removed from the fleet resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-fleet-port-settings-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateFleetPortSettingsInput
---
