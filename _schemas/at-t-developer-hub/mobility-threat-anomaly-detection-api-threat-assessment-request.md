---
description: ThreatAssessmentRequest schema
layout: schema
name: ThreatAssessmentRequest
properties_list:
- description: ''
  name: device
  type: object
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/mobility-threat-anomaly-detection-api-threat-assessment-request-schema.json
slug: mobility-threat-anomaly-detection-api-threat-assessment-request
source_filename: mobility-threat-anomaly-detection-api-threat-assessment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/mobility-threat-anomaly-detection-api-threat-assessment-request-schema.json\",\n  \"title\": \"ThreatAssessmentRequest\",\n  \"description\": \"ThreatAssessmentRequest schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"device\"\n  ],\n  \"properties\": {\n    \"device\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"phoneNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Mobile phone number in E.164 format\",\n          \"example\": \"+12125551234\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/mobility-threat-anomaly-detection-api-threat-assessment-request-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: ThreatAssessmentRequest
---
