---
description: DeleteTimelineEventInput schema
layout: schema
name: DeleteTimelineEventInput
properties_list:
- description: ''
  name: eventId
  type: object
- description: ''
  name: incidentRecordArn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-delete-timeline-event-input-schema.json
slug: incident-manager-delete-timeline-event-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-delete-timeline-event-input-schema.json\",\n  \"title\": \"DeleteTimelineEventInput\",\n  \"description\": \"DeleteTimelineEventInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUID\"\n        },\n        {\n          \"description\": \"The ID of the event to update. You can use <code>ListTimelineEvents</code> to find an event's ID.\"\n        }\n      ]\n    },\n    \"incidentRecordArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the incident that includes the timeline event.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"eventId\"\
  ,\n    \"incidentRecordArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-delete-timeline-event-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: DeleteTimelineEventInput
---
