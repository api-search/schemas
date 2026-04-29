---
description: LogForwardingProfile schema from Palo Alto Networks Strata Logging Service API
layout: schema
name: LogForwardingProfile
properties_list:
- description: Unique identifier of the profile.
  name: profile_id
  type: string
- description: Display name of the profile.
  name: name
  type: string
- description: Description of the profile's purpose.
  name: description
  type: string
- description: Log types included in this forwarding profile.
  name: log_types
  type: array
- description: Whether this profile is actively forwarding logs.
  name: enabled
  type: boolean
- description: Total number of configured destinations.
  name: destination_count
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-logging-service-api-log-forwarding-profile-schema.json
slug: strata-logging-service-api-log-forwarding-profile
source_filename: strata-logging-service-api-log-forwarding-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogForwardingProfile\",\n  \"description\": \"LogForwardingProfile schema from Palo Alto Networks Strata Logging Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-log-forwarding-profile-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profile_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the profile.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the profile.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the profile's purpose.\"\n    },\n    \"log_types\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"traffic\",\n          \"threat\",\n          \"url\",\n    \
  \      \"wildfire\",\n          \"auth\",\n          \"decryption\",\n          \"globalprotect\",\n          \"system\",\n          \"config\"\n        ]\n      },\n      \"description\": \"Log types included in this forwarding profile.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this profile is actively forwarding logs.\"\n    },\n    \"destination_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of configured destinations.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-log-forwarding-profile-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: LogForwardingProfile
---
