---
description: ''
layout: schema
name: RecentEventResponse
properties_list:
- description: ''
  name: recent_event
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-recent-event-response-schema.json
slug: new-relic-recent-event-response
source_filename: new-relic-recent-event-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"recent_event\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"entity_group_id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"entity_id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"entity_type\": {\n          \"type\": \"string\",\n          \"example\": \"standard\"\n        },\n        \"event_type\": {\n          \"type\": \"string\",\n          \"example\": \"standard\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"incident_id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"priority\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"\
  product\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"timestamp\": {\n          \"type\": \"integer\",\n          \"example\": 1718153645993\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecentEventResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-recent-event-response-schema.json
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
title: RecentEventResponse
---
