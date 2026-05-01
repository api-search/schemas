---
description: SearchGameSessionsInput schema from Amazon GameLift API
layout: schema
name: SearchGameSessionsInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: AliasId
  type: object
- description: ''
  name: Location
  type: object
- description: ''
  name: FilterExpression
  type: object
- description: ''
  name: SortExpression
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-search-game-sessions-input-schema.json
slug: gamelift-search-game-sessions-input
source_filename: gamelift-search-game-sessions-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-search-game-sessions-input-schema.json\",\n  \"title\": \"SearchGameSessionsInput\",\n  \"description\": \"SearchGameSessionsInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to search for active game sessions. You can use either the fleet ID or ARN value. Each request must reference either a fleet ID or alias ID, but not both.\"\n        }\n      ]\n    },\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the alias associated with\
  \ the fleet to search for active game sessions. You can use either the alias ID or ARN value. Each request must reference either a fleet ID or alias ID, but not both.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"A fleet location to search for game sessions. You can specify a fleet's home Region or a remote location. Use the Amazon Web Services Region code format, such as <code>us-west-2</code>. \"\n        }\n      ]\n    },\n    \"FilterExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"<p>String containing the search criteria for the session search. If no filter expression is included, the request returns results for all game sessions in the fleet that are in <code>ACTIVE</code> status.</p> <p>A filter expression can\
  \ contain one or multiple conditions. Each condition consists of the following:</p> <ul> <li> <p> <b>Operand</b> -- Name of a game session attribute. Valid values are <code>gameSessionName</code>, <code>gameSessionId</code>, <code>gameSessionProperties</code>, <code>maximumSessions</code>, <code>creationTimeMillis</code>, <code>playerSessionCount</code>, <code>hasAvailablePlayerSessions</code>.</p> </li> <li> <p> <b>Comparator</b> -- Valid comparators are: <code>=</code>, <code>&lt;&gt;</code>, <code>&lt;</code>, <code>&gt;</code>, <code>&lt;=</code>, <code>&gt;=</code>. </p> </li> <li> <p> <b>Value</b> -- Value to be searched for. Values may be numbers, boolean values (true/false) or strings depending on the operand. String values are case sensitive and must be enclosed in single quotes. Special characters must be escaped. Boolean and string values can only be used with the comparators <code>=</code> and <code>&lt;&gt;</code>. For example, the following filter expression searches on <code>gameSessionName</code>:\
  \ \\\"<code>FilterExpression\\\": \\\"gameSessionName = 'Matt\\\\\\\\'s Awesome Game 1'\\\"</code>. </p> </li> </ul> <p>To chain multiple conditions in a single expression, use the logical keywords <code>AND</code>, <code>OR</code>, and <code>NOT</code> and parentheses as needed. For example: <code>x AND y AND NOT z</code>, <code>NOT (x OR y)</code>.</p> <p>Session search evaluates conditions from left to right using the following precedence rules:</p> <ol> <li> <p> <code>=</code>, <code>&lt;&gt;</code>, <code>&lt;</code>, <code>&gt;</code>, <code>&lt;=</code>, <code>&gt;=</code> </p> </li> <li> <p>Parentheses</p> </li> <li> <p>NOT</p> </li> <li> <p>AND</p> </li> <li> <p>OR</p> </li> </ol> <p>For example, this filter expression retrieves game sessions hosting at least ten players that have an open player slot: <code>\\\"maximumSessions&gt;=10 AND hasAvailablePlayerSessions=true\\\"</code>. </p>\"\n        }\n      ]\n    },\n    \"SortExpression\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"<p>Instructions on how to sort the search results. If no sort expression is included, the request returns results in random order. A sort expression consists of the following elements:</p> <ul> <li> <p> <b>Operand</b> -- Name of a game session attribute. Valid values are <code>gameSessionName</code>, <code>gameSessionId</code>, <code>gameSessionProperties</code>, <code>maximumSessions</code>, <code>creationTimeMillis</code>, <code>playerSessionCount</code>, <code>hasAvailablePlayerSessions</code>.</p> </li> <li> <p> <b>Order</b> -- Valid sort orders are <code>ASC</code> (ascending) and <code>DESC</code> (descending).</p> </li> </ul> <p>For example, this sort expression returns the oldest active sessions first: <code>\\\"SortExpression\\\": \\\"creationTimeMillis ASC\\\"</code>. Results with a null value for the sort operand are returned at the end of the list.</p>\"\n  \
  \      }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results to return. Use this parameter with <code>NextToken</code> to get results as a set of sequential pages. The maximum number of results returned is 20, even if this value is not set or is set higher than 20. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates the start of the next sequential page of results. Use the token that is returned with a previous call to this operation. To start at the beginning of the result set, do not specify a value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-search-game-sessions-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: SearchGameSessionsInput
---
