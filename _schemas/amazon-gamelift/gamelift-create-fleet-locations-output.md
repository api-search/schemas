---
description: CreateFleetLocationsOutput schema from Amazon GameLift API
layout: schema
name: CreateFleetLocationsOutput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: FleetArn
  type: object
- description: ''
  name: LocationStates
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-fleet-locations-output-schema.json
slug: gamelift-create-fleet-locations-output
source_filename: gamelift-create-fleet-locations-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-fleet-locations-output-schema.json\",\n  \"title\": \"CreateFleetLocationsOutput\",\n  \"description\": \"CreateFleetLocationsOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet that was updated with new locations.\"\n        }\n      ]\n    },\n    \"FleetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that is assigned to a Amazon GameLift fleet\
  \ resource and uniquely identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::fleet/fleet-a1234567-b8c9-0d1e-2fa3-b45c6d7e8912</code>. \"\n        }\n      ]\n    },\n    \"LocationStates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStateList\"\n        },\n        {\n          \"description\": \"The remote locations that are being added to the fleet, and the life-cycle status of each location. For new locations, the status is set to <code>NEW</code>. During location creation, Amazon GameLift updates each location's status as instances are deployed there and prepared for game hosting. This list does not include the fleet home Region or any remote locations that were already added to the fleet.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-fleet-locations-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateFleetLocationsOutput
---
