---
description: OnboardingStatus schema from Palo Alto Networks SASE Configuration Orchestration API
layout: schema
name: OnboardingStatus
properties_list:
- description: Remote network identifier.
  name: id
  type: string
- description: Current onboarding phase.
  name: status
  type: string
- description: Individual onboarding steps and their completion state.
  name: steps
  type: array
- description: Error description if onboarding failed.
  name: error_message
  type: string
- description: ''
  name: started_at
  type: string
- description: ''
  name: completed_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-config-orchestration-api-onboarding-status-schema.json
slug: sase-config-orchestration-api-onboarding-status
source_filename: sase-config-orchestration-api-onboarding-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OnboardingStatus\",\n  \"description\": \"OnboardingStatus schema from Palo Alto Networks SASE Configuration Orchestration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-onboarding-status-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Remote network identifier.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"provisioning\",\n        \"configuring\",\n        \"tunnel_establishing\",\n        \"completed\",\n        \"failed\"\n      ],\n      \"description\": \"Current onboarding phase.\"\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"Individual onboarding steps and their completion state.\",\n      \"items\": {\n   \
  \     \"type\": \"object\",\n        \"properties\": {\n          \"step\": {\n            \"type\": \"string\",\n            \"description\": \"Step name.\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"pending\",\n              \"in_progress\",\n              \"completed\",\n              \"failed\"\n            ]\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Status message or error detail for this step.\"\n          },\n          \"completed_at\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"error_message\": {\n      \"type\": \"string\",\n      \"description\": \"Error description if onboarding failed.\"\n    },\n    \"started_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\":\
  \ \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-onboarding-status-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: OnboardingStatus
---
