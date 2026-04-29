---
description: A significant event that happened during the incident.
layout: schema
name: TimelineEvent
properties_list:
- description: ''
  name: eventData
  type: object
- description: ''
  name: eventId
  type: object
- description: ''
  name: eventReferences
  type: object
- description: ''
  name: eventTime
  type: object
- description: ''
  name: eventType
  type: object
- description: ''
  name: eventUpdatedTime
  type: object
- description: ''
  name: incidentRecordArn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-timeline-event-schema.json
slug: incident-manager-timeline-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-timeline-event-schema.json\",\n  \"title\": \"TimelineEvent\",\n  \"description\": \"A significant event that happened during the incident. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventData\"\n        },\n        {\n          \"description\": \"A short description of the event.\"\n        }\n      ]\n    },\n    \"eventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUID\"\n        },\n        {\n          \"description\": \"The ID of the timeline event.\"\n        }\n      ]\n    },\n    \"eventReferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventReferenceList\"\n        },\n        {\n        \
  \  \"description\": \"A list of references in a <code>TimelineEvent</code>.\"\n        }\n      ]\n    },\n    \"eventTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the event occurred.\"\n        }\n      ]\n    },\n    \"eventType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimelineEventType\"\n        },\n        {\n          \"description\": \"The type of event that occurred. Currently Incident Manager supports only the <code>Custom Event</code> type.\"\n        }\n      ]\n    },\n    \"eventUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the timeline event was last updated.\"\n        }\n      ]\n    },\n    \"incidentRecordArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the incident that the event occurred during.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"eventData\",\n    \"eventId\",\n    \"eventTime\",\n    \"eventType\",\n    \"eventUpdatedTime\",\n    \"incidentRecordArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-timeline-event-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: TimelineEvent
---
