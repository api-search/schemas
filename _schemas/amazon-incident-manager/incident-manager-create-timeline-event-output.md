---
description: CreateTimelineEventOutput schema
layout: schema
name: CreateTimelineEventOutput
properties_list:
- description: ''
  name: eventId
  type: object
- description: ''
  name: incidentRecordArn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-create-timeline-event-output-schema.json
slug: incident-manager-create-timeline-event-output
source_filename: incident-manager-create-timeline-event-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-create-timeline-event-output-schema.json\",\n  \"title\": \"CreateTimelineEventOutput\",\n  \"description\": \"CreateTimelineEventOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUID\"\n        },\n        {\n          \"description\": \"The ID of the event for easy reference later. \"\n        }\n      ]\n    },\n    \"incidentRecordArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the incident record that you added the event to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"eventId\",\n    \"incidentRecordArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-create-timeline-event-output-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: CreateTimelineEventOutput
---
