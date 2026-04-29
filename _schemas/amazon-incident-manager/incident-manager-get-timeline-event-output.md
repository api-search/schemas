---
description: GetTimelineEventOutput schema
layout: schema
name: GetTimelineEventOutput
properties_list:
- description: ''
  name: event
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-get-timeline-event-output-schema.json
slug: incident-manager-get-timeline-event-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-get-timeline-event-output-schema.json\",\n  \"title\": \"GetTimelineEventOutput\",\n  \"description\": \"GetTimelineEventOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"event\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimelineEvent\"\n        },\n        {\n          \"description\": \"Details about the timeline event.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"event\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-get-timeline-event-output-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: GetTimelineEventOutput
---
