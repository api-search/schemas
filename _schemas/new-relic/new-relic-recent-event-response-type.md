---
description: ''
layout: schema
name: RecentEventResponseType
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: entity_group_id
  type: integer
- description: ''
  name: entity_id
  type: integer
- description: ''
  name: entity_type
  type: string
- description: ''
  name: event_type
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: incident_id
  type: integer
- description: ''
  name: priority
  type: string
- description: ''
  name: product
  type: string
- description: ''
  name: timestamp
  type: integer
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-recent-event-response-type-schema.json
slug: new-relic-recent-event-response-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"entity_group_id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"entity_id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"entity_type\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"event_type\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"incident_id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"product\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"example\": 1718153645993\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"RecentEventResponseType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-recent-event-response-type-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: RecentEventResponseType
---
