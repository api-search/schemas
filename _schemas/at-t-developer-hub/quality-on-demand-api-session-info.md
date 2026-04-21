---
description: SessionInfo schema
layout: schema
name: SessionInfo
properties_list:
- description: Unique identifier for the QoD session
  name: sessionId
  type: string
- description: Device identifier for QoD session
  name: device
  type: object
- description: QoS profile applied to this session
  name: qosProfile
  type: string
- description: Session duration in seconds
  name: duration
  type: integer
- description: Session start timestamp
  name: startedAt
  type: string
- description: Session expiry timestamp
  name: expiresAt
  type: string
- description: Current QoS provisioning status
  name: qosStatus
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/quality-on-demand-api-session-info-schema.json
slug: quality-on-demand-api-session-info
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: SessionInfo
---
