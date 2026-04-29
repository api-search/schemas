---
description: UpdateFleetCapacityInput schema from Amazon GameLift API
layout: schema
name: UpdateFleetCapacityInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: DesiredInstances
  type: object
- description: ''
  name: MinSize
  type: object
- description: ''
  name: MaxSize
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-fleet-capacity-input-schema.json
slug: gamelift-update-fleet-capacity-input
source_filename: gamelift-update-fleet-capacity-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-fleet-capacity-input-schema.json\",\n  \"title\": \"UpdateFleetCapacityInput\",\n  \"description\": \"UpdateFleetCapacityInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to update capacity settings for. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    },\n    \"DesiredInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The number of Amazon EC2 instances you want to maintain in the specified fleet location. This value must fall between\
  \ the minimum and maximum size limits.\"\n        }\n      ]\n    },\n    \"MinSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The minimum number of instances that are allowed in the specified fleet location. If this parameter is not set, the default is 0.\"\n        }\n      ]\n    },\n    \"MaxSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The maximum number of instances that are allowed in the specified fleet location. If this parameter is not set, the default is 1.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"The name of a remote location to update fleet capacity settings for, in the form of an Amazon Web Services Region code\
  \ such as <code>us-west-2</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-fleet-capacity-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateFleetCapacityInput
---
