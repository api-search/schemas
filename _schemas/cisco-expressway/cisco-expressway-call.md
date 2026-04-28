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
