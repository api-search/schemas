---
description: Guidelines for use with FlexMatch to match players into games. All matchmaking requests must specify a matchmaking configuration.
layout: schema
name: MatchmakingConfiguration
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: ConfigurationArn
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: GameSessionQueueArns
  type: object
- description: ''
  name: RequestTimeoutSeconds
  type: object
- description: ''
  name: AcceptanceTimeoutSeconds
  type: object
- description: ''
  name: AcceptanceRequired
  type: object
- description: ''
  name: RuleSetName
  type: object
- description: ''
  name: RuleSetArn
  type: object
- description: ''
  name: NotificationTarget
  type: object
- description: ''
  name: AdditionalPlayerCount
  type: object
- description: ''
  name: CustomEventData
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: GameProperties
  type: object
- description: ''
  name: GameSessionData
  type: object
- description: ''
  name: BackfillMode
  type: object
- description: ''
  name: FlexMatchMode
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-matchmaking-configuration-schema.json
slug: gamelift-matchmaking-configuration
source_filename: gamelift-matchmaking-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-matchmaking-configuration-schema.json\",\n  \"title\": \"MatchmakingConfiguration\",\n  \"description\": \"Guidelines for use with FlexMatch to match players into games. All matchmaking requests must specify a matchmaking configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingIdStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for the matchmaking configuration. This name is used to identify the configuration associated with a matchmaking request or ticket.\"\n        }\n      ]\n    },\n    \"ConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingConfigurationArn\"\n        },\n        {\n     \
  \     \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that is assigned to a Amazon GameLift matchmaking configuration resource and uniquely identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::matchmakingconfiguration/&lt;matchmaking configuration name&gt;</code>. In a Amazon GameLift configuration ARN, the resource ID matches the <i>Name</i> value.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with matchmaking configuration.\"\n        }\n      ]\n    },\n    \"GameSessionQueueArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueueArnsList\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\
  \"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that is assigned to a Amazon GameLift game session queue resource and uniquely identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::gamesessionqueue/&lt;queue name&gt;</code>. Queues can be located in any Region. Queues are used to start new Amazon GameLift-hosted game sessions for matches that are created with this matchmaking configuration. This property is not set when <code>FlexMatchMode</code> is set to <code>STANDALONE</code>.\"\n        }\n      ]\n    },\n    \"RequestTimeoutSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingRequestTimeoutInteger\"\n        },\n        {\n          \"description\": \"The maximum duration, in seconds, that a matchmaking ticket can remain in process before timing out. Requests that fail due to timing out can be resubmitted as needed.\"\n        }\n      ]\n    },\n    \"AcceptanceTimeoutSeconds\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingAcceptanceTimeoutInteger\"\n        },\n        {\n          \"description\": \"The length of time (in seconds) to wait for players to accept a proposed match, if acceptance is required. If any player rejects the match or fails to accept before the timeout, the ticket continues to look for an acceptable match.\"\n        }\n      ]\n    },\n    \"AcceptanceRequired\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanModel\"\n        },\n        {\n          \"description\": \"A flag that indicates whether a match that was created with this configuration must be accepted by the matched players. To require acceptance, set to TRUE. When this option is enabled, matchmaking tickets use the status <code>REQUIRES_ACCEPTANCE</code> to indicate when a completed potential match is waiting for player acceptance.\"\n        }\n      ]\n    },\n    \"RuleSetName\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingIdStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for the matchmaking rule set to use with this configuration. A matchmaking configuration can only use rule sets that are defined in the same Region.\"\n        }\n      ]\n    },\n    \"RuleSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingRuleSetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) associated with the GameLift matchmaking rule set resource that this configuration uses.\"\n        }\n      ]\n    },\n    \"NotificationTarget\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnsArnStringModel\"\n        },\n        {\n          \"description\": \"An SNS topic ARN that is set up to receive matchmaking notifications.\"\
  \n        }\n      ]\n    },\n    \"AdditionalPlayerCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The number of player slots in a match to keep open for future players. For example, if the configuration's rule set specifies a match for a single 12-person team, and the additional player count is set to 2, only 10 players are selected for the match. This parameter is not used when <code>FlexMatchMode</code> is set to <code>STANDALONE</code>.\"\n        }\n      ]\n    },\n    \"CustomEventData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomEventData\"\n        },\n        {\n          \"description\": \"Information to attach to all events related to the matchmaking configuration. \"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n\
  \          \"description\": \"A time stamp indicating when this data object was created. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"GameProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GamePropertyList\"\n        },\n        {\n          \"description\": \"A set of custom properties for a game session, formatted as key:value pairs. These properties are passed to a game server process with a request to start a new game session (see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-api.html#gamelift-sdk-server-startsession\\\">Start a Game Session</a>). This information is added to the new <code>GameSession</code> object that is created for a successful match. This parameter is not used when <code>FlexMatchMode</code> is set to <code>STANDALONE</code>.\"\n        }\n      ]\n    },\n    \"GameSessionData\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionData\"\n        },\n        {\n          \"description\": \"A set of custom game session properties, formatted as a single string value. This data is passed to a game server process with a request to start a new game session (see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-api.html#gamelift-sdk-server-startsession\\\">Start a Game Session</a>). This information is added to the new <code>GameSession</code> object that is created for a successful match. This parameter is not used when <code>FlexMatchMode</code> is set to <code>STANDALONE</code>.\"\n        }\n      ]\n    },\n    \"BackfillMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BackfillMode\"\n        },\n        {\n          \"description\": \"The method used to backfill game sessions created with this matchmaking configuration. MANUAL indicates that the game\
  \ makes backfill requests or does not use the match backfill feature. AUTOMATIC indicates that GameLift creates backfill requests whenever a game session has one or more open slots. Learn more about manual and automatic backfill in <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/flexmatchguide/match-backfill.html\\\">Backfill existing games with FlexMatch</a>. Automatic backfill is not available when <code>FlexMatchMode</code> is set to <code>STANDALONE</code>.\"\n        }\n      ]\n    },\n    \"FlexMatchMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlexMatchMode\"\n        },\n        {\n          \"description\": \"<p>Indicates whether this matchmaking configuration is being used with Amazon GameLift hosting or as a standalone matchmaking solution. </p> <ul> <li> <p> <b>STANDALONE</b> - FlexMatch forms matches and returns match information, including players and team assignments, in a <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/flexmatchguide/match-events.html#match-events-matchmakingsucceeded\\\
  \"> MatchmakingSucceeded</a> event.</p> </li> <li> <p> <b>WITH_QUEUE</b> - FlexMatch forms matches and uses the specified Amazon GameLift queue to start a game session for the match. </p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-matchmaking-configuration-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: MatchmakingConfiguration
---
