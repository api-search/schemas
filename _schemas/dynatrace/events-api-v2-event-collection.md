---
description: A paginated collection of events.
layout: schema
name: EventCollection
properties_list:
- description: The cursor for the next page of results. Null if there are no more pages.
  name: nextPageKey
  type: string
- description: The total number of events matching the query.
  name: totalCount
  type: integer
- description: The number of results returned on this page.
  name: pageSize
  type: integer
- description: The list of events on this page.
  name: events
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/events-api-v2-event-collection-schema.json
slug: events-api-v2-event-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/events-api-v2-event-collection-schema.json\",\n  \"title\": \"EventCollection\",\n  \"description\": \"A paginated collection of events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"The cursor for the next page of results. Null if there are no more pages.\",\n      \"nullable\": true,\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The total number of events matching the query.\",\n      \"example\": 500\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of results returned on this page.\",\n      \"example\": 500\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"\
  description\": \"The list of events on this page.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Event\"\n      },\n      \"example\": [\n        {\n          \"eventId\": \"abc123\",\n          \"eventType\": \"STANDARD\",\n          \"title\": \"example-value\",\n          \"startTime\": 1718153645993,\n          \"endTime\": 1718153645993,\n          \"entityId\": {},\n          \"properties\": {},\n          \"status\": \"OPEN\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/events-api-v2-event-collection-schema.json
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
title: EventCollection
---
