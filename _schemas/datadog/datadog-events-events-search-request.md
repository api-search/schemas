---
description: Request body for searching events using the Events Explorer query language
layout: schema
name: EventsSearchRequest
properties_list:
- description: Filter configuration for the event search
  name: filter
  type: object
- description: Sort order for the returned events
  name: sort
  type: string
- description: Pagination settings for the event search results
  name: page
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-events-events-search-request-schema.json
slug: datadog-events-events-search-request
source_filename: datadog-events-events-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-events-search-request-schema.json\",\n  \"title\": \"EventsSearchRequest\",\n  \"description\": \"Request body for searching events using the Events Explorer query language\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filter\": {\n      \"type\": \"object\",\n      \"description\": \"Filter configuration for the event search\",\n      \"properties\": {\n        \"query\": {\n          \"type\": \"string\",\n          \"description\": \"A Datadog events search query to filter events by text, tags, and attributes\"\n        },\n        \"from\": {\n          \"type\": \"string\",\n          \"description\": \"The start of the search time range as an ISO 8601 timestamp or relative time\"\n        },\n        \"to\": {\n          \"type\": \"string\",\n          \"description\": \"The end\
  \ of the search time range as an ISO 8601 timestamp or relative time\"\n        }\n      }\n    },\n    \"sort\": {\n      \"type\": \"string\",\n      \"description\": \"Sort order for the returned events\",\n      \"enum\": [\n        \"timestamp\",\n        \"-timestamp\"\n      ],\n      \"example\": \"timestamp\"\n    },\n    \"page\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination settings for the event search results\",\n      \"properties\": {\n        \"cursor\": {\n          \"type\": \"string\",\n          \"description\": \"Cursor token from a previous response to retrieve the next page\"\n        },\n        \"limit\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of events to return per page\",\n          \"minimum\": 1,\n          \"maximum\": 1000,\n          \"default\": 10\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-events-search-request-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: EventsSearchRequest
---
