---
description: Schema for a monitored node (network device, server, or virtual machine) in the SolarWinds Orion Platform.
layout: schema
name: SolarWinds Monitored Node
properties_list:
- description: Unique identifier for the node in Orion
  name: NodeID
  type: integer
- description: Display name of the node
  name: Caption
  type: string
- description: Primary IP address of the node
  name: IPAddress
  type: string
- description: GUID representation of the IP address
  name: IPAddressGUID
  type: string
- description: Current monitoring status of the node
  name: Status
  type: integer
- description: Human-readable status description
  name: StatusDescription
  type: string
- description: Type of machine or device
  name: MachineType
  type: string
- description: Hardware or software vendor
  name: Vendor
  type: string
- description: Node sub-type classification
  name: ObjectSubType
  type: string
- description: SNMP sysName value
  name: SysName
  type: string
- description: SNMP sysObjectID value
  name: SysObjectID
  type: string
- description: Physical location of the node
  name: Location
  type: string
- description: Contact person for the node
  name: Contact
  type: string
- description: SNMP community string
  name: Community
  type: string
- description: SNMP version used for polling
  name: SNMPVersion
  type: integer
- description: Polling engine responsible for this node
  name: EngineID
  type: integer
- description: Current CPU utilization percentage
  name: CPULoad
  type: number
- description: Current memory utilization percentage
  name: PercentMemoryUsed
  type: number
- description: Last ICMP response time in milliseconds
  name: ResponseTime
  type: integer
- description: Packet loss percentage
  name: PercentLoss
  type: number
- description: Last boot timestamp
  name: LastBoot
  type: string
- description: Last synchronization timestamp
  name: LastSync
  type: string
- description: SWIS URI for this node entity
  name: Uri
  type: string
- description: Custom properties defined for this node
  name: CustomProperties
  type: object
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-node-schema.json
slug: solarwinds-node
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://solarwinds.com/schemas/solarwinds/node.json\",\n  \"title\": \"SolarWinds Monitored Node\",\n  \"description\": \"Schema for a monitored node (network device, server, or virtual machine) in the SolarWinds Orion Platform.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Caption\",\n    \"IPAddress\"\n  ],\n  \"properties\": {\n    \"NodeID\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the node in Orion\"\n    },\n    \"Caption\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the node\",\n      \"maxLength\": 255\n    },\n    \"IPAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Primary IP address of the node\",\n      \"format\": \"ipv4\"\n    },\n    \"IPAddressGUID\": {\n      \"type\": \"string\",\n      \"description\": \"GUID representation of the IP address\"\n    },\n    \"Status\": {\n      \"\
  type\": \"integer\",\n      \"description\": \"Current monitoring status of the node\",\n      \"enum\": [0, 1, 2, 3, 4, 9, 12, 14, 17, 22],\n      \"examples\": [1]\n    },\n    \"StatusDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable status description\",\n      \"enum\": [\n        \"Unknown\",\n        \"Up\",\n        \"Down\",\n        \"Warning\",\n        \"Shutdown\",\n        \"Unmanaged\",\n        \"Unreachable\",\n        \"Critical\",\n        \"Misconfigured\",\n        \"Could Not Poll\"\n      ]\n    },\n    \"MachineType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of machine or device\"\n    },\n    \"Vendor\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware or software vendor\"\n    },\n    \"ObjectSubType\": {\n      \"type\": \"string\",\n      \"description\": \"Node sub-type classification\",\n      \"enum\": [\n        \"SNMP\",\n        \"ICMP\",\n        \"WMI\",\n        \"Agent\",\n\
  \        \"External\"\n      ]\n    },\n    \"SysName\": {\n      \"type\": \"string\",\n      \"description\": \"SNMP sysName value\"\n    },\n    \"SysObjectID\": {\n      \"type\": \"string\",\n      \"description\": \"SNMP sysObjectID value\"\n    },\n    \"Location\": {\n      \"type\": \"string\",\n      \"description\": \"Physical location of the node\"\n    },\n    \"Contact\": {\n      \"type\": \"string\",\n      \"description\": \"Contact person for the node\"\n    },\n    \"Community\": {\n      \"type\": \"string\",\n      \"description\": \"SNMP community string\"\n    },\n    \"SNMPVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"SNMP version used for polling\",\n      \"enum\": [0, 1, 2, 3]\n    },\n    \"EngineID\": {\n      \"type\": \"integer\",\n      \"description\": \"Polling engine responsible for this node\"\n    },\n    \"CPULoad\": {\n      \"type\": \"number\",\n      \"description\": \"Current CPU utilization percentage\",\n      \"minimum\"\
  : 0,\n      \"maximum\": 100\n    },\n    \"PercentMemoryUsed\": {\n      \"type\": \"number\",\n      \"description\": \"Current memory utilization percentage\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"ResponseTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Last ICMP response time in milliseconds\",\n      \"minimum\": 0\n    },\n    \"PercentLoss\": {\n      \"type\": \"number\",\n      \"description\": \"Packet loss percentage\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"LastBoot\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last boot timestamp\"\n    },\n    \"LastSync\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last synchronization timestamp\"\n    },\n    \"Uri\": {\n      \"type\": \"string\",\n      \"description\": \"SWIS URI for this node entity\"\n    },\n    \"CustomProperties\": {\n      \"type\": \"object\",\n      \"\
  description\": \"Custom properties defined for this node\",\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-node-schema.json
tags:
- Application Monitoring
- Database Monitoring
- Infrastructure
- IP Address Management
- IT Management
- ITSM
- Log Management
- Network Monitoring
- Observability
title: SolarWinds Monitored Node
---
