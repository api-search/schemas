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
schema_file: json-schema/dynatrace-events-v2-event-collection-schema.json
slug: dynatrace-events-v2-event-collection
source_filename: dynatrace-events-v2-event-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A paginated collection of events.\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"The cursor for the next page of results. Null if there are no more pages.\",\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of events matching the query.\",\n      \"format\": \"int64\",\n      \"example\": 500\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of results returned on this page.\",\n      \"example\": 500\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"The list of events on this page.\",\n      \"example\": [\n        {\n          \"eventId\": \"abc123\",\n          \"eventType\": \"STANDARD\",\n          \"title\": \"example-value\",\n          \"startTime\": 1718153645993,\n          \"endTime\": 1718153645993,\n\
  \          \"entityId\": {},\n          \"properties\": {},\n          \"status\": \"OPEN\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a single event in the Dynatrace environment. Events can be ingested via the API or detected automatically by Dynatrace.\",\n        \"properties\": {\n          \"eventId\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the event.\",\n            \"example\": \"abc123\"\n          },\n          \"eventType\": {\n            \"type\": \"string\",\n            \"description\": \"The type of the event.\",\n            \"example\": \"STANDARD\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"description\": \"The display title of the event.\",\n            \"example\": \"example-value\"\n          },\n          \"startTime\": {\n            \"type\": \"integer\",\n            \"description\": \"The start\
  \ time of the event as a Unix timestamp in milliseconds.\",\n            \"format\": \"int64\",\n            \"example\": 1718153645993\n          },\n          \"endTime\": {\n            \"type\": \"integer\",\n            \"description\": \"The end time of the event as a Unix timestamp in milliseconds. Null for open events.\",\n            \"format\": \"int64\",\n            \"example\": 1718153645993\n          },\n          \"entityId\": {\n            \"type\": \"object\",\n            \"description\": \"A lightweight reference to a monitored entity.\",\n            \"properties\": {\n              \"entityId\": {\n                \"type\": \"string\",\n                \"description\": \"The unique identifier of the entity, e.g., SERVICE-1234567890ABCDEF.\",\n                \"example\": \"abc123\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"The display name of the entity.\",\n                \"example\"\
  : \"Production Service\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"The type of the entity, e.g., SERVICE, HOST, PROCESS_GROUP, APPLICATION.\",\n                \"example\": \"STANDARD\"\n              }\n            }\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"Additional key-value metadata attached to the event.\",\n            \"example\": {}\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"The current status of the event. OPEN indicates the event is still active; CLOSED indicates it has ended.\",\n            \"example\": \"OPEN\",\n            \"enum\": [\n              \"OPEN\",\n              \"CLOSED\"\n            ]\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-events-v2-event-collection-schema.json
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
