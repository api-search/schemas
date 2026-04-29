---
description: ThreatIndicator schema
layout: schema
name: ThreatIndicator
properties_list:
- description: Type of threat detected
  name: type
  type: string
- description: Severity of the threat indicator
  name: severity
  type: string
- description: Human-readable description of the threat
  name: description
  type: string
- description: When the threat indicator was detected
  name: detectedAt
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/mobility-threat-anomaly-detection-api-threat-indicator-schema.json
slug: mobility-threat-anomaly-detection-api-threat-indicator
source_filename: mobility-threat-anomaly-detection-api-threat-indicator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/mobility-threat-anomaly-detection-api-threat-indicator-schema.json\",\n  \"title\": \"ThreatIndicator\",\n  \"description\": \"ThreatIndicator schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of threat detected\",\n      \"enum\": [\n        \"UNUSUAL_LOCATION\",\n        \"ABNORMAL_DATA_USAGE\",\n        \"KNOWN_MALWARE_TRAFFIC\",\n        \"SIM_CLONING\",\n        \"ROAMING_ANOMALY\",\n        \"CALL_PATTERN_ANOMALY\"\n      ],\n      \"example\": \"UNUSUAL_LOCATION\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Severity of the threat indicator\",\n      \"enum\": [\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\",\n        \"CRITICAL\"\n      ],\n      \"example\": \"\
  MEDIUM\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the threat\",\n      \"example\": \"Device location changed rapidly from expected home area\"\n    },\n    \"detectedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the threat indicator was detected\",\n      \"example\": \"2026-04-19T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/mobility-threat-anomaly-detection-api-threat-indicator-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: ThreatIndicator
---
