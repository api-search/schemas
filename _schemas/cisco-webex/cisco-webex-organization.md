---
description: Represents a Webex organization containing users, devices, licenses, and configuration settings.
layout: schema
name: Cisco Webex Organization
properties_list:
- description: Unique identifier for the organization.
  name: id
  type: string
- description: Full display name of the organization.
  name: displayName
  type: string
- description: Date and time the organization was created.
  name: created
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-organization-schema.json
slug: cisco-webex-organization
source_filename: cisco-webex-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/organization.json\",\n  \"title\": \"Cisco Webex Organization\",\n  \"description\": \"Represents a Webex organization containing users, devices, licenses, and configuration settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the organization.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name of the organization.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the organization was created.\"\n    }\n  },\n  \"required\": [\"id\", \"displayName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-organization-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Organization
---
