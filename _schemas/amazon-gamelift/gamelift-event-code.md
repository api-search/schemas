---
description: EventCode schema from Amazon GameLift API
layout: schema
name: EventCode
properties_list: []
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-event-code-schema.json
slug: gamelift-event-code
source_filename: gamelift-event-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-event-code-schema.json\",\n  \"title\": \"EventCode\",\n  \"description\": \"EventCode schema from Amazon GameLift API\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"GENERIC_EVENT\",\n    \"FLEET_CREATED\",\n    \"FLEET_DELETED\",\n    \"FLEET_SCALING_EVENT\",\n    \"FLEET_STATE_DOWNLOADING\",\n    \"FLEET_STATE_VALIDATING\",\n    \"FLEET_STATE_BUILDING\",\n    \"FLEET_STATE_ACTIVATING\",\n    \"FLEET_STATE_ACTIVE\",\n    \"FLEET_STATE_ERROR\",\n    \"FLEET_INITIALIZATION_FAILED\",\n    \"FLEET_BINARY_DOWNLOAD_FAILED\",\n    \"FLEET_VALIDATION_LAUNCH_PATH_NOT_FOUND\",\n    \"FLEET_VALIDATION_EXECUTABLE_RUNTIME_FAILURE\",\n    \"FLEET_VALIDATION_TIMED_OUT\",\n    \"FLEET_ACTIVATION_FAILED\",\n    \"FLEET_ACTIVATION_FAILED_NO_INSTANCES\",\n    \"FLEET_NEW_GAME_SESSION_PROTECTION_POLICY_UPDATED\"\
  ,\n    \"SERVER_PROCESS_INVALID_PATH\",\n    \"SERVER_PROCESS_SDK_INITIALIZATION_TIMEOUT\",\n    \"SERVER_PROCESS_PROCESS_READY_TIMEOUT\",\n    \"SERVER_PROCESS_CRASHED\",\n    \"SERVER_PROCESS_TERMINATED_UNHEALTHY\",\n    \"SERVER_PROCESS_FORCE_TERMINATED\",\n    \"SERVER_PROCESS_PROCESS_EXIT_TIMEOUT\",\n    \"GAME_SESSION_ACTIVATION_TIMEOUT\",\n    \"FLEET_CREATION_EXTRACTING_BUILD\",\n    \"FLEET_CREATION_RUNNING_INSTALLER\",\n    \"FLEET_CREATION_VALIDATING_RUNTIME_CONFIG\",\n    \"FLEET_VPC_PEERING_SUCCEEDED\",\n    \"FLEET_VPC_PEERING_FAILED\",\n    \"FLEET_VPC_PEERING_DELETED\",\n    \"INSTANCE_INTERRUPTED\",\n    \"INSTANCE_RECYCLED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-event-code-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: EventCode
---
