---
description: A security event detected by AppOmni in a SaaS application
layout: schema
name: SecurityEvent
properties_list:
- description: Unique security event identifier
  name: eventId
  type: string
- description: Event severity level
  name: severity
  type: string
- description: Type of security event (anomaly, policy-violation, threat, etc.)
  name: type
  type: string
- description: SaaS application where the event occurred
  name: application
  type: string
- description: Human-readable description of the security event
  name: description
  type: string
- description: Timestamp when the event was detected
  name: detectedAt
  type: string
- description: Event investigation status
  name: status
  type: string
- description: User associated with the event
  name: userId
  type: string
provider_name: AppOmni
provider_slug: appomni
schema_file: json-schema/security-event-schema.json
slug: security-event
tags:
- SaaS Security
- Compliance
- Threat Detection
- CASB
- Zero Trust
title: SecurityEvent
---
