---
description: CreateTimelineEventInput schema
layout: schema
name: CreateTimelineEventInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: eventData
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
  name: incidentRecordArn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-create-timeline-event-input-schema.json
slug: incident-manager-create-timeline-event-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-create-timeline-event-input-schema.json\",\n  \"title\": \"CreateTimelineEventInput\",\n  \"description\": \"CreateTimelineEventInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A token that ensures that a client calls the action only once with the specified details.\"\n        }\n      ]\n    },\n    \"eventData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventData\"\n        },\n        {\n          \"description\": \"A short description of the event.\"\n        }\n      ]\n    },\n    \"eventReferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventReferenceList\"\
  \n        },\n        {\n          \"description\": \"Adds one or more references to the <code>TimelineEvent</code>. A reference is an Amazon Web Services resource involved or associated with the incident. To specify a reference, enter its Amazon Resource Name (ARN). You can also specify a related item associated with a resource. For example, to specify an Amazon DynamoDB (DynamoDB) table as a resource, use the table's ARN. You can also specify an Amazon CloudWatch metric associated with the DynamoDB table as a related item.\"\n        }\n      ]\n    },\n    \"eventTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the event occurred.\"\n        }\n      ]\n    },\n    \"eventType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimelineEventType\"\n        },\n        {\n          \"description\": \"The type of event. You can create timeline\
  \ events of type <code>Custom Event</code>.\"\n        }\n      ]\n    },\n    \"incidentRecordArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the incident record that the action adds the incident to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"eventData\",\n    \"eventTime\",\n    \"eventType\",\n    \"incidentRecordArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-create-timeline-event-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: CreateTimelineEventInput
---
