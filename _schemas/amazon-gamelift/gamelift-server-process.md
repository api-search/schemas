---
description: A set of instructions for launching server processes on each instance in a fleet. Server processes run either an executable in a custom game build or a Realtime Servers script. Server process configurations are part of a fleet's runtime configuration.
layout: schema
name: ServerProcess
properties_list:
- description: ''
  name: LaunchPath
  type: object
- description: ''
  name: Parameters
  type: object
- description: ''
  name: ConcurrentExecutions
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-server-process-schema.json
slug: gamelift-server-process
source_filename: gamelift-server-process-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-server-process-schema.json\",\n  \"title\": \"ServerProcess\",\n  \"description\": \"A set of instructions for launching server processes on each instance in a fleet. Server processes run either an executable in a custom game build or a Realtime Servers script. Server process configurations are part of a fleet's runtime configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LaunchPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchPathStringModel\"\n        },\n        {\n          \"description\": \"<p>The location of a game build executable or the Realtime script file that contains the <code>Init()</code> function. Game builds and Realtime scripts are installed on instances at the root: </p> <ul> <li> <p>Windows (custom game builds only):\
  \ <code>C:\\\\game</code>. Example: \\\"<code>C:\\\\game\\\\MyGame\\\\server.exe</code>\\\" </p> </li> <li> <p>Linux: <code>/local/game</code>. Examples: \\\"<code>/local/game/MyGame/server.exe</code>\\\" or \\\"<code>/local/game/MyRealtimeScript.js</code>\\\"</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchParametersStringModel\"\n        },\n        {\n          \"description\": \"An optional list of parameters to pass to the server executable or Realtime script on launch.\"\n        }\n      ]\n    },\n    \"ConcurrentExecutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"The number of server processes using this configuration that run concurrently on each instance.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LaunchPath\",\n    \"ConcurrentExecutions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-server-process-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ServerProcess
---
