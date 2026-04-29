---
description: ThreatSubscription schema
layout: schema
name: ThreatSubscription
properties_list:
- description: Unique subscription identifier
  name: subscriptionId
  type: string
- description: ''
  name: device
  type: object
- description: Minimum risk level triggering notifications
  name: minRiskLevel
  type: string
- description: Subscription status
  name: status
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/mobility-threat-anomaly-detection-api-threat-subscription-schema.json
slug: mobility-threat-anomaly-detection-api-threat-subscription
source_filename: mobility-threat-anomaly-detection-api-threat-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/mobility-threat-anomaly-detection-api-threat-subscription-schema.json\",\n  \"title\": \"ThreatSubscription\",\n  \"description\": \"ThreatSubscription schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subscriptionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique subscription identifier\",\n      \"example\": \"sub-threat-500123\"\n    },\n    \"device\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"phoneNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Mobile phone number in E.164 format\",\n          \"example\": \"+12125551234\"\n        }\n      }\n    },\n    \"minRiskLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Minimum risk level triggering notifications\",\n      \"example\": \"MEDIUM\"\n    },\n\
  \    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription status\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\"\n      ],\n      \"example\": \"ACTIVE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/mobility-threat-anomaly-detection-api-threat-subscription-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: ThreatSubscription
---
