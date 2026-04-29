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
source_filename: mobility-threat-anomaly-detection-api-threat-subscription-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/mobility-threat-anomaly-detection-api-threat-subscription-request-schema.json\",\n  \"title\": \"ThreatSubscriptionRequest\",\n  \"description\": \"ThreatSubscriptionRequest schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"device\",\n    \"notificationUrl\"\n  ],\n  \"properties\": {\n    \"device\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"phoneNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Mobile phone number in E.164 format\",\n          \"example\": \"+12125551234\"\n        }\n      }\n    },\n    \"notificationUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Webhook URL for threat alert notifications\",\n      \"example\": \"https://webhook.example.com/threats\"\n    },\n    \"minRiskLevel\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Minimum risk level to trigger notifications\",\n      \"enum\": [\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\",\n        \"CRITICAL\"\n      ],\n      \"example\": \"MEDIUM\"\n    },\n    \"notificationAuthToken\": {\n      \"type\": \"string\",\n      \"description\": \"Bearer token for webhook authentication\",\n      \"example\": \"webhook-token-abc123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/mobility-threat-anomaly-detection-api-threat-subscription-request-schema.json
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
