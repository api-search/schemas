---
description: Information about AwsGroundStationAgentEndpoint.
layout: schema
name: AwsGroundStationAgentEndpoint
properties_list:
- description: ''
  name: agentStatus
  type: object
- description: ''
  name: auditResults
  type: object
- description: ''
  name: egressAddress
  type: object
- description: ''
  name: ingressAddress
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-aws-ground-station-agent-endpoint-schema.json
slug: ground-station-aws-ground-station-agent-endpoint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-aws-ground-station-agent-endpoint-schema.json\",\n  \"title\": \"AwsGroundStationAgentEndpoint\",\n  \"description\": \"Information about AwsGroundStationAgentEndpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgentStatus\"\n        },\n        {\n          \"description\": \"The status of AgentEndpoint.\"\n        }\n      ]\n    },\n    \"auditResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditResults\"\n        },\n        {\n          \"description\": \"The results of the audit.\"\n        }\n      ]\n    },\n    \"egressAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionDetails\"\n  \
  \      },\n        {\n          \"description\": \"The egress address of AgentEndpoint.\"\n        }\n      ]\n    },\n    \"ingressAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RangedConnectionDetails\"\n        },\n        {\n          \"description\": \"The ingress address of AgentEndpoint.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SafeName\"\n        },\n        {\n          \"description\": \"Name string associated with AgentEndpoint. Used as a human-readable identifier for AgentEndpoint.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"egressAddress\",\n    \"ingressAddress\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-aws-ground-station-agent-endpoint-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: AwsGroundStationAgentEndpoint
---
