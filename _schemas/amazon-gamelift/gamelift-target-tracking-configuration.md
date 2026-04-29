---
description: <p> <b>This data type is used with the Amazon GameLift FleetIQ and game server groups.</b> </p> <p>Settings for a target-based scaling policy as part of a <a href="https://docs.aws.amazon.com/gamelift/latest/apireference/API_GameServerGroupAutoScalingPolicy.html">GameServerGroupAutoScalingPolicy</a> . These settings are used to create a target-based policy that tracks the Amazon GameLift FleetIQ metric <code>"PercentUtilizedGameServers"</code> and specifies a target value for the metric. As player usage changes, the policy triggers to adjust the game server group capacity so that the metric returns to the target value. </p>
layout: schema
name: TargetTrackingConfiguration
properties_list:
- description: ''
  name: TargetValue
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-target-tracking-configuration-schema.json
slug: gamelift-target-tracking-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-target-tracking-configuration-schema.json\",\n  \"title\": \"TargetTrackingConfiguration\",\n  \"description\": \"<p> <b>This data type is used with the Amazon GameLift FleetIQ and game server groups.</b> </p> <p>Settings for a target-based scaling policy as part of a <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_GameServerGroupAutoScalingPolicy.html\\\">GameServerGroupAutoScalingPolicy</a> . These settings are used to create a target-based policy that tracks the Amazon GameLift FleetIQ metric <code>\\\"PercentUtilizedGameServers\\\"</code> and specifies a target value for the metric. As player usage changes, the policy triggers to adjust the game server group capacity so that the metric returns to the target value. </p>\",\n  \"type\": \"object\",\n  \"properties\"\
  : {\n    \"TargetValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonNegativeDouble\"\n        },\n        {\n          \"description\": \"Desired value to use with a game server group target-based scaling policy. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TargetValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-target-tracking-configuration-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: TargetTrackingConfiguration
---
