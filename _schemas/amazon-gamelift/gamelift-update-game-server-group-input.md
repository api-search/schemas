---
description: UpdateGameServerGroupInput schema from Amazon GameLift API
layout: schema
name: UpdateGameServerGroupInput
properties_list:
- description: ''
  name: GameServerGroupName
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: InstanceDefinitions
  type: object
- description: ''
  name: GameServerProtectionPolicy
  type: object
- description: ''
  name: BalancingStrategy
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-game-server-group-input-schema.json
slug: gamelift-update-game-server-group-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-game-server-group-input-schema.json\",\n  \"title\": \"UpdateGameServerGroupInput\",\n  \"description\": \"UpdateGameServerGroupInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupNameOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the game server group. Use either the name or ARN value.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) for an\
  \ IAM role that allows Amazon GameLift to access your Amazon EC2 Auto Scaling groups.\"\n        }\n      ]\n    },\n    \"InstanceDefinitions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceDefinitions\"\n        },\n        {\n          \"description\": \"An updated list of Amazon EC2 instance types to use in the Auto Scaling group. The instance definitions must specify at least two different instance types that are supported by Amazon GameLift FleetIQ. This updated list replaces the entire current list of instance definitions for the game server group. For more information on instance types, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-types.html\\\">EC2 Instance Types</a> in the <i>Amazon EC2 User Guide</i>. You can optionally specify capacity weighting for each instance type. If no weight value is specified for an instance type, it is set to the default value \\\"1\\\". For more information about capacity weighting,\
  \ see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/asg-instance-weighting.html\\\"> Instance Weighting for Amazon EC2 Auto Scaling</a> in the Amazon EC2 Auto Scaling User Guide.\"\n        }\n      ]\n    },\n    \"GameServerProtectionPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerProtectionPolicy\"\n        },\n        {\n          \"description\": \"A flag that indicates whether instances in the game server group are protected from early termination. Unprotected instances that have active game servers running might be terminated during a scale-down event, causing players to be dropped from the game. Protected instances cannot be terminated while there are active game servers running except in the event of a forced game server group deletion (see ). An exception to this is with Spot Instances, which can be terminated by Amazon Web Services regardless of protection status. This property is set to <code>NO_PROTECTION</code>\
  \ by default.\"\n        }\n      ]\n    },\n    \"BalancingStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BalancingStrategy\"\n        },\n        {\n          \"description\": \"<p>Indicates how Amazon GameLift FleetIQ balances the use of Spot Instances and On-Demand Instances in the game server group. Method options include the following:</p> <ul> <li> <p> <code>SPOT_ONLY</code> - Only Spot Instances are used in the game server group. If Spot Instances are unavailable or not viable for game hosting, the game server group provides no hosting capacity until Spot Instances can again be used. Until then, no new instances are started, and the existing nonviable Spot Instances are terminated (after current gameplay ends) and are not replaced.</p> </li> <li> <p> <code>SPOT_PREFERRED</code> - (default value) Spot Instances are used whenever available in the game server group. If Spot Instances are unavailable, the game server group continues to provide\
  \ hosting capacity by falling back to On-Demand Instances. Existing nonviable Spot Instances are terminated (after current gameplay ends) and are replaced with new On-Demand Instances.</p> </li> <li> <p> <code>ON_DEMAND_ONLY</code> - Only On-Demand Instances are used in the game server group. No Spot Instances are used, even when available, while this balancing strategy is in force.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GameServerGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-game-server-group-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateGameServerGroupInput
---
