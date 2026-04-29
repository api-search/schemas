---
description: Detailed information about the agent.
layout: schema
name: AgentDetails
properties_list:
- description: ''
  name: agentCpuCores
  type: object
- description: ''
  name: agentVersion
  type: object
- description: ''
  name: componentVersions
  type: object
- description: ''
  name: instanceId
  type: object
- description: ''
  name: instanceType
  type: object
- description: ''
  name: reservedCpuCores
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-agent-details-schema.json
slug: ground-station-agent-details
source_filename: ground-station-agent-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-agent-details-schema.json\",\n  \"title\": \"AgentDetails\",\n  \"description\": \"Detailed information about the agent.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentCpuCores\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgentCpuCoresList\"\n        },\n        {\n          \"description\": \"List of CPU cores reserved for the agent.\"\n        }\n      ]\n    },\n    \"agentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionString\"\n        },\n        {\n          \"description\": \"Current agent version.\"\n        }\n      ]\n    },\n    \"componentVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionList\"\n        },\n        {\n \
  \         \"description\": \"List of versions being used by agent components.\"\n        }\n      ]\n    },\n    \"instanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceId\"\n        },\n        {\n          \"description\": \"ID of EC2 instance agent is running on.\"\n        }\n      ]\n    },\n    \"instanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceType\"\n        },\n        {\n          \"description\": \"Type of EC2 instance agent is running on.\"\n        }\n      ]\n    },\n    \"reservedCpuCores\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgentCpuCoresList\"\n        },\n        {\n          \"description\": \"<note> <p>This field should not be used. Use agentCpuCores instead.</p> </note> <p>List of CPU cores reserved for processes other than the agent running on the EC2 instance.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"agentVersion\"\
  ,\n    \"componentVersions\",\n    \"instanceId\",\n    \"instanceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-agent-details-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: AgentDetails
---
