---
description: Ticket generated to track the progress of a matchmaking request. Each ticket is uniquely identified by a ticket ID, supplied by the requester, when creating a matchmaking request.
layout: schema
name: MatchmakingTicket
properties_list:
- description: ''
  name: TicketId
  type: object
- description: ''
  name: ConfigurationName
  type: object
- description: ''
  name: ConfigurationArn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusReason
  type: object
- description: ''
  name: StatusMessage
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: Players
  type: object
- description: ''
  name: GameSessionConnectionInfo
  type: object
- description: ''
  name: EstimatedWaitTime
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-matchmaking-ticket-schema.json
slug: gamelift-matchmaking-ticket
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-matchmaking-ticket-schema.json\",\n  \"title\": \"MatchmakingTicket\",\n  \"description\": \"Ticket generated to track the progress of a matchmaking request. Each ticket is uniquely identified by a ticket ID, supplied by the requester, when creating a matchmaking request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TicketId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingIdStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for a matchmaking ticket.\"\n        }\n      ]\n    },\n    \"ConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingIdStringModel\"\n        },\n        {\n          \"description\": \"Name of the matchmaking configuration that is\
  \ used with this ticket. Matchmaking configurations determine how players are grouped into a match and how a new game session is created for the match.\"\n        }\n      ]\n    },\n    \"ConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingConfigurationArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) associated with the GameLift matchmaking configuration resource that is used with this ticket.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingConfigurationStatus\"\n        },\n        {\n          \"description\": \"<p>Current status of the matchmaking request.</p> <ul> <li> <p> <b>QUEUED</b> -- The matchmaking request has been received and is currently waiting to be processed.</p> </li> <li> <p> <b>SEARCHING</b> -- The\
  \ matchmaking request is currently being processed. </p> </li> <li> <p> <b>REQUIRES_ACCEPTANCE</b> -- A match has been proposed and the players must accept the match. This status is used only with requests that use a matchmaking configuration with a player acceptance requirement.</p> </li> <li> <p> <b>PLACING</b> -- The FlexMatch engine has matched players and is in the process of placing a new game session for the match.</p> </li> <li> <p> <b>COMPLETED</b> -- Players have been matched and a game session is ready to host the players. A ticket in this state contains the necessary connection information for players.</p> </li> <li> <p> <b>FAILED</b> -- The matchmaking request was not completed.</p> </li> <li> <p> <b>CANCELLED</b> -- The matchmaking request was canceled. This may be the result of a <code>StopMatchmaking</code> operation or a proposed match that one or more players failed to accept.</p> </li> <li> <p> <b>TIMED_OUT</b> -- The matchmaking request was not successful within the\
  \ duration specified in the matchmaking configuration. </p> </li> </ul> <note> <p>Matchmaking requests that fail to successfully complete (statuses FAILED, CANCELLED, TIMED_OUT) can be resubmitted as new requests with new ticket IDs.</p> </note>\"\n        }\n      ]\n    },\n    \"StatusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringModel\"\n        },\n        {\n          \"description\": \"Code to explain the current status. For example, a status reason may indicate when a ticket has returned to <code>SEARCHING</code> status after a proposed match fails to receive player acceptances.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringModel\"\n        },\n        {\n          \"description\": \"Additional information about the current status.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"Time stamp indicating when this matchmaking request was received. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Time stamp indicating when the matchmaking request stopped being processed due to successful completion, timeout, or cancellation. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"Players\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerList\"\n        },\n        {\n          \"description\": \"A set of <code>Player</code> objects, each representing a player to find matches for. Players are identified by a unique player ID and may include latency\
  \ data for use during matchmaking. If the ticket is in status <code>COMPLETED</code>, the <code>Player</code> objects include the team the players were assigned to in the resulting match.\"\n        }\n      ]\n    },\n    \"GameSessionConnectionInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionConnectionInfo\"\n        },\n        {\n          \"description\": \"Connection information for a new game session. Once a match is made, the FlexMatch engine creates a new game session for it. This information is added to the matchmaking ticket, which you can be retrieve by calling <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_DescribeMatchmaking.html\\\">DescribeMatchmaking</a> .\"\n        }\n      ]\n    },\n    \"EstimatedWaitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"Average amount of time (in seconds) that players\
  \ are currently waiting for a match. If there is not enough recent data, this property may be empty.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-matchmaking-ticket-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: MatchmakingTicket
---
