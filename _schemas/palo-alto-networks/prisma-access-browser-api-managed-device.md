---
description: ManagedDevice schema from Palo Alto Networks Prisma Access Browser Management API
layout: schema
name: ManagedDevice
properties_list:
- description: Unique identifier of the managed device.
  name: device_id
  type: string
- description: Device hostname.
  name: hostname
  type: string
- description: Operating system platform.
  name: platform
  type: string
- description: Installed Prisma Access Browser version.
  name: browser_version
  type: string
- description: Device compliance status.
  name: compliance_status
  type: string
- description: ID of the last user who logged in on this device.
  name: user_id
  type: string
- description: Timestamp of the device's last check-in.
  name: last_seen_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-browser-api-managed-device-schema.json
slug: prisma-access-browser-api-managed-device
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedDevice\",\n  \"description\": \"ManagedDevice schema from Palo Alto Networks Prisma Access Browser Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-managed-device-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"device_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the managed device.\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Device hostname.\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"windows\",\n        \"macos\",\n        \"linux\",\n        \"chromeos\"\n      ],\n      \"description\": \"Operating system platform.\"\n    },\n    \"browser_version\": {\n      \"type\": \"string\",\n      \"description\": \"Installed Prisma Access Browser\
  \ version.\"\n    },\n    \"compliance_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"compliant\",\n        \"non_compliant\",\n        \"unknown\"\n      ],\n      \"description\": \"Device compliance status.\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the last user who logged in on this device.\"\n    },\n    \"last_seen_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the device's last check-in.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-managed-device-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ManagedDevice
---
