---
description: CreateSessionRequest schema
layout: schema
name: CreateSessionRequest
properties_list:
- description: Device identifier for QoD session
  name: device
  type: object
- description: Requested QoS profile
  name: qosProfile
  type: string
- description: Session duration in seconds (default and max vary by profile)
  name: duration
  type: integer
- description: Webhook URL to receive QoS status change notifications
  name: notificationUrl
  type: string
- description: Bearer token for webhook notification authentication
  name: notificationAuthToken
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/quality-on-demand-api-create-session-request-schema.json
slug: quality-on-demand-api-create-session-request
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: CreateSessionRequest
---
