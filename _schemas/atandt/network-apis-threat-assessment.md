---
description: ML-based device threat assessment from AT&T network
layout: schema
name: Threat Assessment
properties_list:
- description: ''
  name: riskLevel
  type: string
- description: ''
  name: anomalyScore
  type: number
- description: ''
  name: threats
  type: array
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/network-apis-threat-assessment-schema.json
slug: network-apis-threat-assessment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/network/threat-assessment\",\n  \"title\": \"Threat Assessment\",\n  \"description\": \"ML-based device threat assessment from AT&T network\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"riskLevel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\",\n        \"CRITICAL\"\n      ]\n    },\n    \"anomalyScore\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1\n    },\n    \"threats\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"UNUSUAL_LOCATION\",\n          \"ABNORMAL_DATA_USAGE\",\n          \"KNOWN_MALWARE_TRAFFIC\",\n          \"SIM_CLONING\",\n          \"ROAMING_ANOMALY\",\n          \"CALL_PATTERN_ANOMALY\"\n        ]\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/network-apis-threat-assessment-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Threat Assessment
---
