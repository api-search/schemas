---
description: A range of IP addresses and port settings that allow inbound traffic to connect to server processes on an instance in a fleet. New game sessions are assigned an IP address/port number combination, which must fall into the fleet's allowed ranges. Fleets with custom game builds must have permissions explicitly set. For Realtime Servers fleets, Amazon GameLift automatically opens two port ranges, one for TCP messaging and one for UDP.
layout: schema
name: IpPermission
properties_list:
- description: ''
  name: FromPort
  type: object
- description: ''
  name: ToPort
  type: object
- description: ''
  name: IpRange
  type: object
- description: ''
  name: Protocol
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-ip-permission-schema.json
slug: gamelift-ip-permission
source_filename: gamelift-ip-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-ip-permission-schema.json\",\n  \"title\": \"IpPermission\",\n  \"description\": \"A range of IP addresses and port settings that allow inbound traffic to connect to server processes on an instance in a fleet. New game sessions are assigned an IP address/port number combination, which must fall into the fleet's allowed ranges. Fleets with custom game builds must have permissions explicitly set. For Realtime Servers fleets, Amazon GameLift automatically opens two port ranges, one for TCP messaging and one for UDP.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FromPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"<p>A starting value for a range of allowed port numbers.</p> <p>For fleets\
  \ using Linux builds, only ports <code>22</code> and <code>1026-60000</code> are valid.</p> <p>For fleets using Windows builds, only ports <code>1026-60000</code> are valid.</p>\"\n        }\n      ]\n    },\n    \"ToPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"<p>An ending value for a range of allowed port numbers. Port numbers are end-inclusive. This value must be equal to or greater than <code>FromPort</code>.</p> <p>For fleets using Linux builds, only ports <code>22</code> and <code>1026-60000</code> are valid.</p> <p>For fleets using Windows builds, only ports <code>1026-60000</code> are valid.</p>\"\n        }\n      ]\n    },\n    \"IpRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonBlankString\"\n        },\n        {\n          \"description\": \"A range of allowed IP addresses. This value must be expressed in CIDR notation. Example:\
  \ \\\"<code>000.000.000.000/[subnet mask]</code>\\\" or optionally the shortened version \\\"<code>0.0.0.0/[subnet mask]</code>\\\".\"\n        }\n      ]\n    },\n    \"Protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpProtocol\"\n        },\n        {\n          \"description\": \"The network communication protocol used by the fleet.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FromPort\",\n    \"ToPort\",\n    \"IpRange\",\n    \"Protocol\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-ip-permission-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: IpPermission
---
