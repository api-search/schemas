---
description: Configuration for a game session placement mechanism that processes requests for new game sessions. A queue can be used on its own or as part of a matchmaking solution.
layout: schema
name: GameSessionQueue
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: GameSessionQueueArn
  type: object
- description: ''
  name: TimeoutInSeconds
  type: object
- description: ''
  name: PlayerLatencyPolicies
  type: object
- description: ''
  name: Destinations
  type: object
- description: ''
  name: FilterConfiguration
  type: object
- description: ''
  name: PriorityConfiguration
  type: object
- description: ''
  name: CustomEventData
  type: object
- description: ''
  name: NotificationTarget
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-game-session-queue-schema.json
slug: gamelift-game-session-queue
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-session-queue-schema.json\",\n  \"title\": \"GameSessionQueue\",\n  \"description\": \"Configuration for a game session placement mechanism that processes requests for new game sessions. A queue can be used on its own or as part of a matchmaking solution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionQueueName\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with game session queue. Queue names must be unique within each Region.\"\n        }\n      ]\n    },\n    \"GameSessionQueueArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionQueueArn\"\n        },\n        {\n          \"description\": \"The\
  \ Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that is assigned to a Amazon GameLift game session queue resource and uniquely identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::gamesessionqueue/&lt;queue name&gt;</code>. In a Amazon GameLift game session queue ARN, the resource ID matches the <i>Name</i> value.\"\n        }\n      ]\n    },\n    \"TimeoutInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The maximum time, in seconds, that a new game session placement request remains in the queue. When a request exceeds this time, the game session placement changes to a <code>TIMED_OUT</code> status.\"\n        }\n      ]\n    },\n    \"PlayerLatencyPolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerLatencyPolicyList\"\n  \
  \      },\n        {\n          \"description\": \"A set of policies that act as a sliding cap on player latency. FleetIQ works to deliver low latency for most players in a game session. These policies ensure that no individual player can be placed into a game with unreasonably high latency. Use multiple policies to gradually relax latency requirements a step at a time. Multiple policies are applied based on their maximum allowed latency, starting with the lowest value. \"\n        }\n      ]\n    },\n    \"Destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionQueueDestinationList\"\n        },\n        {\n          \"description\": \"A list of fleets and/or fleet aliases that can be used to fulfill game session placement requests in the queue. Destinations are identified by either a fleet ARN or a fleet alias ARN, and are listed in order of placement preference.\"\n        }\n      ]\n    },\n    \"FilterConfiguration\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/FilterConfiguration\"\n        },\n        {\n          \"description\": \"A list of locations where a queue is allowed to place new game sessions. Locations are specified in the form of Amazon Web Services Region codes, such as <code>us-west-2</code>. If this parameter is not set, game sessions can be placed in any queue location. \"\n        }\n      ]\n    },\n    \"PriorityConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PriorityConfiguration\"\n        },\n        {\n          \"description\": \"Custom settings to use when prioritizing destinations and locations for game session placements. This configuration replaces the FleetIQ default prioritization process. Priority types that are not explicitly named will be automatically applied at the end of the prioritization process. \"\n        }\n      ]\n    },\n    \"CustomEventData\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/QueueCustomEventData\"\n        },\n        {\n          \"description\": \" Information that is added to all events that are related to this game session queue.\"\n        }\n      ]\n    },\n    \"NotificationTarget\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueueSnsArnStringModel\"\n        },\n        {\n          \"description\": \"An SNS topic ARN that is set up to receive game session placement notifications. See <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/queue-notification.html\\\"> Setting up notifications for game session placement</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-session-queue-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GameSessionQueue
---
