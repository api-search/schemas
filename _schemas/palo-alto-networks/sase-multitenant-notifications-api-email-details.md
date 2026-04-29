---
description: EmailDetails schema from Multi-Tenant Notifications API
layout: schema
name: EmailDetails
properties_list:
- description: Email owner name
  name: name
  type: string
- description: Email id
  name: emailId
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-email-details-schema.json
slug: sase-multitenant-notifications-api-email-details
source_filename: sase-multitenant-notifications-api-email-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailDetails\",\n  \"description\": \"EmailDetails schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-email-details-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Email owner name\",\n      \"type\": \"string\"\n    },\n    \"emailId\": {\n      \"description\": \"Email id\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"emailId\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-email-details-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: EmailDetails
---
