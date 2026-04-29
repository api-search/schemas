---
description: Response containing a paginated list of events from the Events Explorer
layout: schema
name: EventsListResponse
properties_list:
- description: List of event objects matching the search criteria
  name: data
  type: array
- description: Pagination links for navigating through the result set
  name: links
  type: object
- description: Metadata about the event list response
  name: meta
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-events-events-list-response-schema.json
slug: datadog-events-events-list-response
source_filename: datadog-events-events-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-events-list-response-schema.json\",\n  \"title\": \"EventsListResponse\",\n  \"description\": \"Response containing a paginated list of events from the Events Explorer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"List of event objects matching the search criteria\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Event\"\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination links for navigating through the result set\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"string\",\n          \"description\": \"URL for the next page of results; absent if this is the last page\"\n        }\n      }\n    },\n    \"meta\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Metadata about the event list response\",\n      \"properties\": {\n        \"page\": {\n          \"type\": \"object\",\n          \"description\": \"Pagination cursor information for this response\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor token to pass in the next request to retrieve the next page of results\"\n            }\n          }\n        },\n        \"elapsed\": {\n          \"type\": \"integer\",\n          \"description\": \"Time in milliseconds taken to process the event search query\"\n        },\n        \"request_id\": {\n          \"type\": \"string\",\n          \"description\": \"A unique identifier for this search request, useful for debugging\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The completion status of the search request\",\n          \"enum\": [\n            \"done\",\n          \
  \  \"timeout\"\n          ]\n        },\n        \"warnings\": {\n          \"type\": \"array\",\n          \"description\": \"List of non-fatal warning messages about the search query or results\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-events-list-response-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: EventsListResponse
---
