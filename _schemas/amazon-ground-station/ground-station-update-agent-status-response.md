---
description: UpdateAgentStatusResponse schema from Amazon Ground Station API
layout: schema
name: UpdateAgentStatusResponse
properties_list:
- description: ''
  name: agentId
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-update-agent-status-response-schema.json
slug: ground-station-update-agent-status-response
source_filename: ground-station-update-agent-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-update-agent-status-response-schema.json\",\n  \"title\": \"UpdateAgentStatusResponse\",\n  \"description\": \"UpdateAgentStatusResponse schema from Amazon Ground Station API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"UUID of updated agent.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"agentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-update-agent-status-response-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: UpdateAgentStatusResponse
---
