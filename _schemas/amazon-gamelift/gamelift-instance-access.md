---
description: Information required to remotely connect to a fleet instance.
layout: schema
name: InstanceAccess
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: InstanceId
  type: object
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: OperatingSystem
  type: object
- description: ''
  name: Credentials
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-instance-access-schema.json
slug: gamelift-instance-access
source_filename: gamelift-instance-access-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-instance-access-schema.json\",\n  \"title\": \"InstanceAccess\",\n  \"description\": \"Information required to remotely connect to a fleet instance. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetId\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet containing the instance being accessed.\"\n        }\n      ]\n    },\n    \"InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceId\"\n        },\n        {\n          \"description\": \"A unique identifier for the instance being accessed.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddress\"\
  \n        },\n        {\n          \"description\": \"IP address that is assigned to the instance.\"\n        }\n      ]\n    },\n    \"OperatingSystem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OperatingSystem\"\n        },\n        {\n          \"description\": \"Operating system that is running on the instance.\"\n        }\n      ]\n    },\n    \"Credentials\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceCredentials\"\n        },\n        {\n          \"description\": \"Credentials required to access the instance.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-instance-access-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: InstanceAccess
---
