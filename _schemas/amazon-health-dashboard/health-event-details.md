---
description: Detailed information about an event. A combination of an <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_Event.html">Event</a> object, an <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_EventDescription.html">EventDescription</a> object, and additional metadata about the event. Returned by the <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventDetails.html">DescribeEventDetails</a> operation.
layout: schema
name: EventDetails
properties_list:
- description: ''
  name: event
  type: object
- description: ''
  name: eventDescription
  type: object
- description: ''
  name: eventMetadata
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-event-details-schema.json
slug: health-event-details
source_filename: health-event-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-details-schema.json\",\n  \"title\": \"EventDetails\",\n  \"description\": \"Detailed information about an event. A combination of an <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_Event.html\\\">Event</a> object, an <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_EventDescription.html\\\">EventDescription</a> object, and additional metadata about the event. Returned by the <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventDetails.html\\\">DescribeEventDetails</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"event\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Event\"\n        },\n        {\n          \"description\": \"Summary information about the\
  \ event.\"\n        }\n      ]\n    },\n    \"eventDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventDescription\"\n        },\n        {\n          \"description\": \"The most recent description of the event.\"\n        }\n      ]\n    },\n    \"eventMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventMetadata\"\n        },\n        {\n          \"description\": \"Additional metadata about the event.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-details-schema.json
tags:
- Health Monitoring
- Notifications
- Operations
- Service Status
title: EventDetails
---
