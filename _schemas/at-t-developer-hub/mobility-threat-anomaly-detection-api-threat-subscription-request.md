---
description: ThreatSubscriptionRequest schema
layout: schema
name: ThreatSubscriptionRequest
properties_list:
- description: ''
  name: device
  type: object
- description: Webhook URL for threat alert notifications
  name: notificationUrl
  type: string
- description: Minimum risk level to trigger notifications
  name: minRiskLevel
  type: string
- description: Bearer token for webhook authentication
  name: notificationAuthToken
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/mobility-threat-anomaly-detection-api-threat-subscription-request-schema.json
slug: mobility-threat-anomaly-detection-api-threat-subscription-request
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: ThreatSubscriptionRequest
---
