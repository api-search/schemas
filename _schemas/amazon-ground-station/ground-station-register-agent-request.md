---
description: RegisterAgentRequest schema from Amazon Ground Station API
layout: schema
name: RegisterAgentRequest
properties_list:
- description: ''
  name: agentDetails
  type: object
- description: ''
  name: discoveryData
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-register-agent-request-schema.json
slug: ground-station-register-agent-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-register-agent-request-schema.json\",\n  \"title\": \"RegisterAgentRequest\",\n  \"description\": \"RegisterAgentRequest schema from Amazon Ground Station API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgentDetails\"\n        },\n        {\n          \"description\": \"Detailed information about the agent being registered.\"\n        }\n      ]\n    },\n    \"discoveryData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiscoveryData\"\n        },\n        {\n          \"description\": \"Data for associating an agent with the capabilities it is managing.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"agentDetails\",\n    \"discoveryData\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-register-agent-request-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: RegisterAgentRequest
---
