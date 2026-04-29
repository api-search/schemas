---
description: Schema for a call record on Cisco Expressway. Represents both active calls and completed call history records. Call history is limited to the most recent 500 calls, or fewer if calls used multiple components. Calls may be SIP, H.323, or interworked between protocols.
layout: schema
name: Cisco Expressway Call
properties_list:
- description: Unique identifier for the call
  name: CallId
  type: string
- description: ISO 8601 timestamp when the call started, referenced to NTP time
  name: StartTime
  type: string
- description: ISO 8601 timestamp when the call ended. Null for active calls.
  name: EndTime
  type:
  - string
  - 'null'
- description: Call duration in seconds. For active calls, this is the current elapsed time.
  name: Duration
  type: integer
- description: Alias of the calling endpoint or the transformed source identifier
  name: SourceAlias
  type: string
- description: Alias of the called endpoint or the transformed destination identifier
  name: DestinationAlias
  type: string
- description: Type of call based on the signaling protocol(s) involved
  name: CallType
  type: string
- description: SIP variant for SIP-based calls, indicating the specific SIP dialect used
  name: SIPVariant
  type: string
- description: Protocols involved in the call. May indicate single or multiple protocol components.
  name: Protocol
  type: string
- description: Call outcome or current state
  name: Status
  type: string
- description: Reason for call disconnection. Only present for completed calls.
  name: DisconnectReason
  type: string
- description: Bandwidth usage in kbps. For active calls, this is the current bandwidth.
  name: Bandwidth
  type: integer
- description: Zone where the call originated
  name: SourceZone
  type: string
- description: Zone where the call terminates
  name: DestinationZone
  type: string
- description: Whether media encryption is active for this call
  name: Encrypted
  type: boolean
- description: Identifier of the cluster node handling this call
  name: ClusterPeer
  type: string
provider_name: Cisco Expressway
provider_slug: cisco-expressway
schema_file: json-schema/cisco-expressway-call-schema.json
slug: cisco-expressway-call
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/cisco-expressway/json-schema/cisco-expressway-call-schema.json\",\n  \"title\": \"Cisco Expressway Call\",\n  \"description\": \"Schema for a call record on Cisco Expressway. Represents both active calls and completed call history records. Call history is limited to the most recent 500 calls, or fewer if calls used multiple components. Calls may be SIP, H.323, or interworked between protocols.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CallId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the call\"\n    },\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the call started, referenced to NTP time\"\n    },\n    \"EndTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601\
  \ timestamp when the call ended. Null for active calls.\"\n    },\n    \"Duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Call duration in seconds. For active calls, this is the current elapsed time.\",\n      \"minimum\": 0\n    },\n    \"SourceAlias\": {\n      \"type\": \"string\",\n      \"description\": \"Alias of the calling endpoint or the transformed source identifier\",\n      \"examples\": [\"user1@example.com\", \"+14155551234\"]\n    },\n    \"DestinationAlias\": {\n      \"type\": \"string\",\n      \"description\": \"Alias of the called endpoint or the transformed destination identifier\",\n      \"examples\": [\"user2@example.com\", \"meeting@example.com\"]\n    },\n    \"CallType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of call based on the signaling protocol(s) involved\",\n      \"enum\": [\"SIP\", \"H.323\", \"Interworked\"]\n    },\n    \"SIPVariant\": {\n      \"type\": \"string\",\n      \"description\": \"SIP variant for\
  \ SIP-based calls, indicating the specific SIP dialect used\",\n      \"enum\": [\"Standard\", \"Microsoft AV\", \"Microsoft SIP IM&P\"]\n    },\n    \"Protocol\": {\n      \"type\": \"string\",\n      \"description\": \"Protocols involved in the call. May indicate single or multiple protocol components.\",\n      \"examples\": [\"SIP\", \"H.323\", \"SIP/H.323\"]\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Call outcome or current state\",\n      \"examples\": [\"Active\", \"Completed\", \"Failed\", \"Rejected\"]\n    },\n    \"DisconnectReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for call disconnection. Only present for completed calls.\"\n    },\n    \"Bandwidth\": {\n      \"type\": \"integer\",\n      \"description\": \"Bandwidth usage in kbps. For active calls, this is the current bandwidth.\",\n      \"minimum\": 0\n    },\n    \"SourceZone\": {\n      \"type\": \"string\",\n      \"description\": \"Zone where the\
  \ call originated\",\n      \"examples\": [\"LocalZone\", \"CEtoEXPE-Traversal\"]\n    },\n    \"DestinationZone\": {\n      \"type\": \"string\",\n      \"description\": \"Zone where the call terminates\",\n      \"examples\": [\"CUCM-Neighbor\", \"DefaultDNSZone\"]\n    },\n    \"Encrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether media encryption is active for this call\"\n    },\n    \"ClusterPeer\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the cluster node handling this call\"\n    }\n  },\n  \"required\": [\"CallId\", \"StartTime\", \"SourceAlias\", \"DestinationAlias\", \"CallType\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/json-schema/cisco-expressway-call-schema.json
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
title: Cisco Expressway Call
---
