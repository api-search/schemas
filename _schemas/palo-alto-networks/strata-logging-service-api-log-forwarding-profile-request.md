---
description: LogForwardingProfileRequest schema from Palo Alto Networks Strata Logging Service API
layout: schema
name: LogForwardingProfileRequest
properties_list:
- description: Display name for the profile.
  name: name
  type: string
- description: Optional description.
  name: description
  type: string
- description: Log types to include in forwarding.
  name: log_types
  type: array
- description: ''
  name: enabled
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-logging-service-api-log-forwarding-profile-request-schema.json
slug: strata-logging-service-api-log-forwarding-profile-request
source_filename: strata-logging-service-api-log-forwarding-profile-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogForwardingProfileRequest\",\n  \"description\": \"LogForwardingProfileRequest schema from Palo Alto Networks Strata Logging Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-log-forwarding-profile-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the profile.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description.\"\n    },\n    \"log_types\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"traffic\",\n          \"threat\",\n          \"url\",\n          \"wildfire\",\n          \"auth\",\n          \"decryption\",\n          \"globalprotect\",\n          \"system\"\
  ,\n          \"config\"\n        ]\n      },\n      \"description\": \"Log types to include in forwarding.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"log_types\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-log-forwarding-profile-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: LogForwardingProfileRequest
---
