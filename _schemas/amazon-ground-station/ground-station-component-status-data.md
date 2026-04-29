---
description: Data on the status of agent components.
layout: schema
name: ComponentStatusData
properties_list:
- description: ''
  name: bytesReceived
  type: object
- description: ''
  name: bytesSent
  type: object
- description: ''
  name: capabilityArn
  type: object
- description: ''
  name: componentType
  type: object
- description: ''
  name: dataflowId
  type: object
- description: ''
  name: packetsDropped
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-component-status-data-schema.json
slug: ground-station-component-status-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-component-status-data-schema.json\",\n  \"title\": \"ComponentStatusData\",\n  \"description\": \"Data on the status of agent components.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bytesReceived\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"Bytes received by the component.\"\n        }\n      ]\n    },\n    \"bytesSent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"Bytes sent by the component.\"\n        }\n      ]\n    },\n    \"capabilityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapabilityArn\"\n        },\n        {\n          \"description\"\
  : \"Capability ARN of the component.\"\n        }\n      ]\n    },\n    \"componentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentTypeString\"\n        },\n        {\n          \"description\": \"The Component type.\"\n        }\n      ]\n    },\n    \"dataflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"Dataflow UUID associated with the component.\"\n        }\n      ]\n    },\n    \"packetsDropped\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"Packets dropped by component.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgentStatus\"\n        },\n        {\n          \"description\": \"Component status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"capabilityArn\"\
  ,\n    \"componentType\",\n    \"dataflowId\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-component-status-data-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: ComponentStatusData
---
