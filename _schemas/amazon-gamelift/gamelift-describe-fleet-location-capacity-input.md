---
description: DescribeFleetLocationCapacityInput schema from Amazon GameLift API
layout: schema
name: DescribeFleetLocationCapacityInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-fleet-location-capacity-input-schema.json
slug: gamelift-describe-fleet-location-capacity-input
source_filename: gamelift-describe-fleet-location-capacity-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-fleet-location-capacity-input-schema.json\",\n  \"title\": \"DescribeFleetLocationCapacityInput\",\n  \"description\": \"DescribeFleetLocationCapacityInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to request location capacity for. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"The fleet location to retrieve capacity information for. Specify a location in the\
  \ form of an Amazon Web Services Region code, such as <code>us-west-2</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\",\n    \"Location\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-fleet-location-capacity-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeFleetLocationCapacityInput
---
