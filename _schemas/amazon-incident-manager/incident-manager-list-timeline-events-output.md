---
description: ListTimelineEventsOutput schema
layout: schema
name: ListTimelineEventsOutput
properties_list:
- description: ''
  name: eventSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-list-timeline-events-output-schema.json
slug: incident-manager-list-timeline-events-output
source_filename: incident-manager-list-timeline-events-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-timeline-events-output-schema.json\",\n  \"title\": \"ListTimelineEventsOutput\",\n  \"description\": \"ListTimelineEventsOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventSummaryList\"\n        },\n        {\n          \"description\": \"Details about each event that occurred during the incident.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token to continue to the next page of results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"eventSummaries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-timeline-events-output-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: ListTimelineEventsOutput
---
