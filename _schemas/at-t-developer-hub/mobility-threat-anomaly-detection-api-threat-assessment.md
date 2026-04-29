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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/mobility-threat-anomaly-detection-api-threat-assessment-schema.json\",\n  \"title\": \"ThreatAssessment\",\n  \"description\": \"ThreatAssessment schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"riskLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Overall risk level for the device\",\n      \"enum\": [\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\",\n        \"CRITICAL\"\n      ],\n      \"example\": \"LOW\"\n    },\n    \"anomalyScore\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Normalized anomaly score from 0.0 (normal) to 1.0 (highly anomalous)\",\n      \"minimum\": 0.0,\n      \"maximum\": 1.0,\n      \"example\": 0.05\n    },\n    \"threats\": {\n      \"type\": \"array\",\n      \"description\": \"List of detected\
  \ threat indicators\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Type of threat detected\",\n            \"enum\": [\n              \"UNUSUAL_LOCATION\",\n              \"ABNORMAL_DATA_USAGE\",\n              \"KNOWN_MALWARE_TRAFFIC\",\n              \"SIM_CLONING\",\n              \"ROAMING_ANOMALY\",\n              \"CALL_PATTERN_ANOMALY\"\n            ],\n            \"example\": \"UNUSUAL_LOCATION\"\n          },\n          \"severity\": {\n            \"type\": \"string\",\n            \"description\": \"Severity of the threat indicator\",\n            \"enum\": [\n              \"LOW\",\n              \"MEDIUM\",\n              \"HIGH\",\n              \"CRITICAL\"\n            ],\n            \"example\": \"MEDIUM\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable description of\
  \ the threat\",\n            \"example\": \"Device location changed rapidly from expected home area\"\n          },\n          \"detectedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"When the threat indicator was detected\",\n            \"example\": \"2026-04-19T14:30:00Z\"\n          }\n        }\n      }\n    },\n    \"assessedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the threat assessment\",\n      \"example\": \"2026-04-19T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/mobility-threat-anomaly-detection-api-threat-assessment-schema.json
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
