---
description: UpdateAgentStatusRequest schema from Amazon Ground Station API
layout: schema
name: UpdateAgentStatusRequest
properties_list:
- description: ''
  name: aggregateStatus
  type: object
- description: ''
  name: componentStatuses
  type: object
- description: ''
  name: taskId
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-update-agent-status-request-schema.json
slug: ground-station-update-agent-status-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-update-agent-status-request-schema.json\",\n  \"title\": \"UpdateAgentStatusRequest\",\n  \"description\": \"UpdateAgentStatusRequest schema from Amazon Ground Station API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"aggregateStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregateStatus\"\n        },\n        {\n          \"description\": \"Aggregate status for agent.\"\n        }\n      ]\n    },\n    \"componentStatuses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentStatusList\"\n        },\n        {\n          \"description\": \"List of component statuses for agent.\"\n        }\n      ]\n    },\n    \"taskId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\
  \n        },\n        {\n          \"description\": \"GUID of agent task.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"aggregateStatus\",\n    \"componentStatuses\",\n    \"taskId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-update-agent-status-request-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: UpdateAgentStatusRequest
---
