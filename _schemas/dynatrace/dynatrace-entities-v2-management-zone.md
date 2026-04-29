---
description: A management zone reference.
layout: schema
name: ManagementZone
properties_list:
- description: The unique identifier of the management zone.
  name: id
  type: string
- description: The display name of the management zone.
  name: name
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-entities-v2-management-zone-schema.json
slug: dynatrace-entities-v2-management-zone
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A management zone reference.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the management zone.\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the management zone.\",\n      \"example\": \"Production Service\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagementZone\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-entities-v2-management-zone-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: ManagementZone
---
