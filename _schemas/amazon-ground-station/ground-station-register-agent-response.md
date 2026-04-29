---
description: RegisterAgentResponse schema from Amazon Ground Station API
layout: schema
name: RegisterAgentResponse
properties_list:
- description: ''
  name: agentId
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-register-agent-response-schema.json
slug: ground-station-register-agent-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-register-agent-response-schema.json\",\n  \"title\": \"RegisterAgentResponse\",\n  \"description\": \"RegisterAgentResponse schema from Amazon Ground Station API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"UUID of registered agent.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-register-agent-response-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: RegisterAgentResponse
---
