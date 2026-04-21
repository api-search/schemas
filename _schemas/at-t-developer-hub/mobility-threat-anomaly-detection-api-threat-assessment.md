---
description: ThreatAssessment schema
layout: schema
name: ThreatAssessment
properties_list:
- description: Overall risk level for the device
  name: riskLevel
  type: string
- description: Normalized anomaly score from 0.0 (normal) to 1.0 (highly anomalous)
  name: anomalyScore
  type: number
- description: List of detected threat indicators
  name: threats
  type: array
- description: Timestamp of the threat assessment
  name: assessedAt
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/mobility-threat-anomaly-detection-api-threat-assessment-schema.json
slug: mobility-threat-anomaly-detection-api-threat-assessment
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: ThreatAssessment
---
