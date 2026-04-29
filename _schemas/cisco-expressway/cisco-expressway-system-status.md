---
description: Schema for the system status overview of a Cisco Expressway node. Includes system identification, software and hardware versions, network configuration, resource usage, cluster role, and option key status.
layout: schema
name: Cisco Expressway System Status
properties_list:
- description: The name assigned to the Expressway node
  name: SystemName
  type: string
- description: Currently installed software version
  name: SoftwareVersion
  type: string
- description: Hardware appliance version or VM designation
  name: HardwareVersion
  type: string
- description: Hardware or VM serial number used for identification and licensing
  name: SerialNumber
  type: string
- description: Time elapsed since the system last restarted, in human-readable format
  name: Uptime
  type: string
- description: IPv4 address of the Expressway node
  name: IPv4Address
  type: string
- description: IPv6 address of the Expressway node, if configured
  name: IPv6Address
  type:
  - string
  - 'null'
- description: Virtual machine size designation which determines capacity limits
  name: VMSize
  type: string
- description: Number of devices currently registered with this Expressway node
  name: CurrentRegistrations
  type: integer
- description: Number of calls currently active on this Expressway node
  name: CurrentCalls
  type: integer
- description: Role of this node in a cluster configuration
  name: ClusterRole
  type: string
- description: List of installed option keys and their activation status
  name: OptionKeys
  type: array
provider_name: Cisco Expressway
provider_slug: cisco-expressway
schema_file: json-schema/cisco-expressway-system-status-schema.json
slug: cisco-expressway-system-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/cisco-expressway/json-schema/cisco-expressway-system-status-schema.json\",\n  \"title\": \"Cisco Expressway System Status\",\n  \"description\": \"Schema for the system status overview of a Cisco Expressway node. Includes system identification, software and hardware versions, network configuration, resource usage, cluster role, and option key status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SystemName\": {\n      \"type\": \"string\",\n      \"description\": \"The name assigned to the Expressway node\",\n      \"examples\": [\"Expressway-C-Primary\", \"Expressway-E-Edge\"]\n    },\n    \"SoftwareVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Currently installed software version\",\n      \"examples\": [\"X14.2\", \"X15.0\"]\n    },\n    \"HardwareVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware appliance\
  \ version or VM designation\",\n      \"examples\": [\"VM\", \"CE1200\"]\n    },\n    \"SerialNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware or VM serial number used for identification and licensing\"\n    },\n    \"Uptime\": {\n      \"type\": \"string\",\n      \"description\": \"Time elapsed since the system last restarted, in human-readable format\",\n      \"examples\": [\"45 days 12:34:56\", \"2 days 03:15:42\"]\n    },\n    \"IPv4Address\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"IPv4 address of the Expressway node\",\n      \"examples\": [\"10.0.0.1\"]\n    },\n    \"IPv6Address\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"ipv6\",\n      \"description\": \"IPv6 address of the Expressway node, if configured\"\n    },\n    \"VMSize\": {\n      \"type\": \"string\",\n      \"description\": \"Virtual machine size designation which determines capacity limits\",\n      \"enum\": [\"Small\"\
  , \"Medium\", \"Large\"]\n    },\n    \"CurrentRegistrations\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of devices currently registered with this Expressway node\",\n      \"minimum\": 0,\n      \"examples\": [150]\n    },\n    \"CurrentCalls\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of calls currently active on this Expressway node\",\n      \"minimum\": 0,\n      \"examples\": [12]\n    },\n    \"ClusterRole\": {\n      \"type\": \"string\",\n      \"description\": \"Role of this node in a cluster configuration\",\n      \"enum\": [\"Primary\", \"Peer\", \"Standalone\"]\n    },\n    \"OptionKeys\": {\n      \"type\": \"array\",\n      \"description\": \"List of installed option keys and their activation status\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Name\": {\n            \"type\": \"string\",\n            \"description\": \"Feature or capacity option key name\",\n            \"examples\"\
  : [\"Rich Media Sessions\", \"Advanced Networking\"]\n          },\n          \"Status\": {\n            \"type\": \"string\",\n            \"description\": \"Activation status of the option key\",\n            \"enum\": [\"Active\", \"Expired\", \"Not Installed\"]\n          }\n        },\n        \"required\": [\"Name\", \"Status\"]\n      }\n    }\n  },\n  \"required\": [\"SystemName\", \"SoftwareVersion\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/json-schema/cisco-expressway-system-status-schema.json
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
title: Cisco Expressway System Status
---
