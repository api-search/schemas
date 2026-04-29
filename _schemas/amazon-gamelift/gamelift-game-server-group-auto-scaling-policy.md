---
description: <p> <b>This data type is used with the Amazon GameLift FleetIQ and game server groups.</b> </p> <p>Configuration settings for intelligent automatic scaling that uses target tracking. These settings are used to add an Auto Scaling policy when creating the corresponding Auto Scaling group. After the Auto Scaling group is created, all updates to Auto Scaling policies, including changing this policy and adding or removing other policies, is done directly on the Auto Scaling group. </p>
layout: schema
name: GameServerGroupAutoScalingPolicy
properties_list:
- description: ''
  name: EstimatedInstanceWarmup
  type: object
- description: ''
  name: TargetTrackingConfiguration
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-game-server-group-auto-scaling-policy-schema.json
slug: gamelift-game-server-group-auto-scaling-policy
source_filename: gamelift-game-server-group-auto-scaling-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-server-group-auto-scaling-policy-schema.json\",\n  \"title\": \"GameServerGroupAutoScalingPolicy\",\n  \"description\": \"<p> <b>This data type is used with the Amazon GameLift FleetIQ and game server groups.</b> </p> <p>Configuration settings for intelligent automatic scaling that uses target tracking. These settings are used to add an Auto Scaling policy when creating the corresponding Auto Scaling group. After the Auto Scaling group is created, all updates to Auto Scaling policies, including changing this policy and adding or removing other policies, is done directly on the Auto Scaling group. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EstimatedInstanceWarmup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n\
  \        {\n          \"description\": \"Length of time, in seconds, it takes for a new instance to start new game server processes and register with Amazon GameLift FleetIQ. Specifying a warm-up time can be useful, particularly with game servers that take a long time to start up, because it avoids prematurely starting new instances. \"\n        }\n      ]\n    },\n    \"TargetTrackingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetTrackingConfiguration\"\n        },\n        {\n          \"description\": \"Settings for a target-based scaling policy applied to Auto Scaling group. These settings are used to create a target-based policy that tracks the Amazon GameLift FleetIQ metric <code>\\\"PercentUtilizedGameServers\\\"</code> and specifies a target value for the metric. As player usage changes, the policy triggers to adjust the game server group capacity so that the metric returns to the target value. \"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"TargetTrackingConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-server-group-auto-scaling-policy-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GameServerGroupAutoScalingPolicy
---
