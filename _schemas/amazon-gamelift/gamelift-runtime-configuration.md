---
description: <p>A collection of server process configurations that describe the set of processes to run on each instance in a fleet. Server processes run either an executable in a custom game build or a Realtime Servers script. Amazon GameLift launches the configured processes, manages their life cycle, and replaces them as needed. Each instance checks regularly for an updated runtime configuration. </p> <p>A Amazon GameLift instance is limited to 50 processes running concurrently. To calculate the total number of processes in a runtime configuration, add the values of the <code>ConcurrentExecutions</code> parameter for each server process. Learn more about <a href="https://docs.aws.amazon.com/gamelift/latest/developerguide/fleets-multiprocess.html"> Running Multiple Processes on a Fleet</a>.</p>
layout: schema
name: RuntimeConfiguration
properties_list:
- description: ''
  name: ServerProcesses
  type: object
- description: ''
  name: MaxConcurrentGameSessionActivations
  type: object
- description: ''
  name: GameSessionActivationTimeoutSeconds
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-runtime-configuration-schema.json
slug: gamelift-runtime-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-runtime-configuration-schema.json\",\n  \"title\": \"RuntimeConfiguration\",\n  \"description\": \"<p>A collection of server process configurations that describe the set of processes to run on each instance in a fleet. Server processes run either an executable in a custom game build or a Realtime Servers script. Amazon GameLift launches the configured processes, manages their life cycle, and replaces them as needed. Each instance checks regularly for an updated runtime configuration. </p> <p>A Amazon GameLift instance is limited to 50 processes running concurrently. To calculate the total number of processes in a runtime configuration, add the values of the <code>ConcurrentExecutions</code> parameter for each server process. Learn more about <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/fleets-multiprocess.html\\\
  \"> Running Multiple Processes on a Fleet</a>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServerProcesses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerProcessList\"\n        },\n        {\n          \"description\": \"A collection of server process configurations that identify what server processes to run on each instance in a fleet.\"\n        }\n      ]\n    },\n    \"MaxConcurrentGameSessionActivations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxConcurrentGameSessionActivations\"\n        },\n        {\n          \"description\": \"The number of game sessions in status <code>ACTIVATING</code> to allow on an instance. This setting limits the instance resources that can be used for new game activations at any one time.\"\n        }\n      ]\n    },\n    \"GameSessionActivationTimeoutSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionActivationTimeoutSeconds\"\
  \n        },\n        {\n          \"description\": \"The maximum amount of time (in seconds) allowed to launch a new game session and have it report ready to host players. During this time, the game session is in status <code>ACTIVATING</code>. If the game session does not become active before the timeout, it is ended and the game session status is changed to <code>TERMINATED</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-runtime-configuration-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: RuntimeConfiguration
---
