---
description: <p> <b>This data type is used with the Amazon GameLift FleetIQ and game server groups.</b> </p> <p>Properties that describe a game server group resource. A game server group manages certain properties related to a corresponding Amazon EC2 Auto Scaling group. </p> <p>A game server group is created by a successful call to <code>CreateGameServerGroup</code> and deleted by calling <code>DeleteGameServerGroup</code>. Game server group activity can be temporarily suspended and resumed by calling <code>SuspendGameServerGroup</code> and <code>ResumeGameServerGroup</code>, respectively. </p>
layout: schema
name: GameServerGroup
properties_list:
- description: ''
  name: GameServerGroupName
  type: object
- description: ''
  name: GameServerGroupArn
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: InstanceDefinitions
  type: object
- description: ''
  name: BalancingStrategy
  type: object
- description: ''
  name: GameServerProtectionPolicy
  type: object
- description: ''
  name: AutoScalingGroupArn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusReason
  type: object
- description: ''
  name: SuspendedActions
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-game-server-group-schema.json
slug: gamelift-game-server-group
source_filename: gamelift-game-server-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-server-group-schema.json\",\n  \"title\": \"GameServerGroup\",\n  \"description\": \"<p> <b>This data type is used with the Amazon GameLift FleetIQ and game server groups.</b> </p> <p>Properties that describe a game server group resource. A game server group manages certain properties related to a corresponding Amazon EC2 Auto Scaling group. </p> <p>A game server group is created by a successful call to <code>CreateGameServerGroup</code> and deleted by calling <code>DeleteGameServerGroup</code>. Game server group activity can be temporarily suspended and resumed by calling <code>SuspendGameServerGroup</code> and <code>ResumeGameServerGroup</code>, respectively. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroupName\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/GameServerGroupName\"\n        },\n        {\n          \"description\": \"A developer-defined identifier for the game server group. The name is unique for each Region in each Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"GameServerGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupArn\"\n        },\n        {\n          \"description\": \"A generated unique ID for the game server group.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) for an IAM role that allows Amazon GameLift to access your Amazon EC2 Auto Scaling groups.\"\n        }\n      ]\n    },\n    \"InstanceDefinitions\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/InstanceDefinitions\"\n        },\n        {\n          \"description\": \"The set of Amazon EC2 instance types that Amazon GameLift FleetIQ can use when balancing and automatically scaling instances in the corresponding Auto Scaling group. \"\n        }\n      ]\n    },\n    \"BalancingStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BalancingStrategy\"\n        },\n        {\n          \"description\": \"<p>Indicates how Amazon GameLift FleetIQ balances the use of Spot Instances and On-Demand Instances in the game server group. Method options include the following:</p> <ul> <li> <p> <code>SPOT_ONLY</code> - Only Spot Instances are used in the game server group. If Spot Instances are unavailable or not viable for game hosting, the game server group provides no hosting capacity until Spot Instances can again be used. Until then, no new instances are started, and the existing nonviable Spot Instances are terminated (after\
  \ current gameplay ends) and are not replaced.</p> </li> <li> <p> <code>SPOT_PREFERRED</code> - (default value) Spot Instances are used whenever available in the game server group. If Spot Instances are unavailable, the game server group continues to provide hosting capacity by falling back to On-Demand Instances. Existing nonviable Spot Instances are terminated (after current gameplay ends) and are replaced with new On-Demand Instances.</p> </li> <li> <p> <code>ON_DEMAND_ONLY</code> - Only On-Demand Instances are used in the game server group. No Spot Instances are used, even when available, while this balancing strategy is in force.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"GameServerProtectionPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerProtectionPolicy\"\n        },\n        {\n          \"description\": \"A flag that indicates whether instances in the game server group are protected from early termination. Unprotected\
  \ instances that have active game servers running might be terminated during a scale-down event, causing players to be dropped from the game. Protected instances cannot be terminated while there are active game servers running except in the event of a forced game server group deletion (see ). An exception to this is with Spot Instances, which can be terminated by Amazon Web Services regardless of protection status. \"\n        }\n      ]\n    },\n    \"AutoScalingGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupArn\"\n        },\n        {\n          \"description\": \"A generated unique ID for the Amazon EC2 Auto Scaling group that is associated with this game server group.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupStatus\"\n        },\n        {\n          \"description\": \"<p>The current status of the game server group. Possible statuses\
  \ include:</p> <ul> <li> <p> <code>NEW</code> - Amazon GameLift FleetIQ has validated the <code>CreateGameServerGroup()</code> request. </p> </li> <li> <p> <code>ACTIVATING</code> - Amazon GameLift FleetIQ is setting up a game server group, which includes creating an Auto Scaling group in your Amazon Web Services account. </p> </li> <li> <p> <code>ACTIVE</code> - The game server group has been successfully created. </p> </li> <li> <p> <code>DELETE_SCHEDULED</code> - A request to delete the game server group has been received. </p> </li> <li> <p> <code>DELETING</code> - Amazon GameLift FleetIQ has received a valid <code>DeleteGameServerGroup()</code> request and is processing it. Amazon GameLift FleetIQ must first complete and release hosts before it deletes the Auto Scaling group and the game server group. </p> </li> <li> <p> <code>DELETED</code> - The game server group has been successfully deleted. </p> </li> <li> <p> <code>ERROR</code> - The asynchronous processes of activating or deleting\
  \ a game server group has failed, resulting in an error state.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"StatusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"Additional information about the current game server group status. This information might provide additional insight on groups that are in <code>ERROR</code> status.\"\n        }\n      ]\n    },\n    \"SuspendedActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupActions\"\n        },\n        {\n          \"description\": \"A list of activities that are currently suspended for this game server group. If this property is empty, all activities are occurring.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A time stamp\
  \ indicating when this data object was created. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp that indicates when this game server group was last updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-server-group-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GameServerGroup
---
