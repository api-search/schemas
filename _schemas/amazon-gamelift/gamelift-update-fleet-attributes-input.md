---
description: UpdateFleetAttributesInput schema from Amazon GameLift API
layout: schema
name: UpdateFleetAttributesInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: NewGameSessionProtectionPolicy
  type: object
- description: ''
  name: ResourceCreationLimitPolicy
  type: object
- description: ''
  name: MetricGroups
  type: object
- description: ''
  name: AnywhereConfiguration
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-fleet-attributes-input-schema.json
slug: gamelift-update-fleet-attributes-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-fleet-attributes-input-schema.json\",\n  \"title\": \"UpdateFleetAttributesInput\",\n  \"description\": \"UpdateFleetAttributesInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to update attribute metadata for. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with a fleet. Fleet names do not need to be unique.\"\n        }\n   \
  \   ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A human-readable description of a fleet.\"\n        }\n      ]\n    },\n    \"NewGameSessionProtectionPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProtectionPolicy\"\n        },\n        {\n          \"description\": \"<p>The game session protection policy to apply to all new instances created in this fleet. Instances that already exist are not affected. You can set protection for individual instances using <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_UpdateGameSession.html\\\">UpdateGameSession</a> .</p> <ul> <li> <p> <b>NoProtection</b> -- The game session can be terminated during a scale-down event.</p> </li> <li> <p> <b>FullProtection</b> -- If the game session is in an <code>ACTIVE</code> status, it cannot be terminated during\
  \ a scale-down event.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ResourceCreationLimitPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCreationLimitPolicy\"\n        },\n        {\n          \"description\": \"Policy settings that limit the number of game sessions an individual player can create over a span of time. \"\n        }\n      ]\n    },\n    \"MetricGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricGroupList\"\n        },\n        {\n          \"description\": \"The name of a metric group to add this fleet to. Use a metric group in Amazon CloudWatch to aggregate the metrics from multiple fleets. Provide an existing metric group name, or create a new metric group by providing a new name. A fleet can only be in one metric group at a time.\"\n        }\n      ]\n    },\n    \"AnywhereConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnywhereConfiguration\"\
  \n        },\n        {\n          \"description\": \"Amazon GameLift Anywhere configuration options.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-fleet-attributes-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateFleetAttributesInput
---
