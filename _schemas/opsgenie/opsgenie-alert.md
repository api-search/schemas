---
description: Represents an alert in the OpsGenie incident management platform. Alerts are the primary mechanism for notifying teams about issues that require attention.
layout: schema
name: OpsGenie Alert
properties_list:
- description: Unique identifier of the alert assigned by OpsGenie.
  name: id
  type: string
- description: Short, human-readable identifier for the alert.
  name: tinyId
  type: string
- description: Client-defined identifier used for alert deduplication.
  name: alias
  type: string
- description: The alert message, limited to 130 characters.
  name: message
  type: string
- description: Detailed description providing context about the alert.
  name: description
  type: string
- description: Current status of the alert.
  name: status
  type: string
- description: Whether the alert has been acknowledged by a responder.
  name: acknowledged
  type: boolean
- description: Whether the alert has been viewed.
  name: isSeen
  type: boolean
- description: Whether the alert is currently snoozed.
  name: snoozed
  type: boolean
- description: Date and time when the snooze period ends.
  name: snoozedUntil
  type: string
- description: Tags attached to the alert for categorization.
  name: tags
  type: array
- description: Number of times the alert has occurred (deduplication count).
  name: count
  type: integer
- description: Date and time of the most recent occurrence.
  name: lastOccurredAt
  type: string
- description: Date and time when the alert was first created.
  name: createdAt
  type: string
- description: Date and time of the last modification.
  name: updatedAt
  type: string
- description: Source of the alert, typically the integration or tool that created it.
  name: source
  type: string
- description: Username of the alert owner (assigned user).
  name: owner
  type: string
- description: Priority level from P1 (critical) to P5 (informational).
  name: priority
  type: string
- description: Entity field used to specify the domain of the alert.
  name: entity
  type: string
- description: Teams, users, escalations, and schedules responsible for the alert.
  name: responders
  type: array
- description: Teams and users who can see the alert without receiving notifications.
  name: visibleTo
  type: array
- description: Custom actions available for the alert.
  name: actions
  type: array
- description: Custom key-value pairs providing additional context.
  name: details
  type: object
- description: ''
  name: integration
  type: object
- description: ''
  name: report
  type: object
provider_name: OpsGenie
provider_slug: opsgenie
schema_file: json-schema/opsgenie-alert-schema.json
slug: opsgenie-alert
source_filename: opsgenie-alert-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api-evangelist.com/opsgenie/alert.json\",\n  \"title\": \"OpsGenie Alert\",\n  \"description\": \"Represents an alert in the OpsGenie incident management platform. Alerts are the primary mechanism for notifying teams about issues that require attention.\",\n  \"type\": \"object\",\n  \"required\": [\"message\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the alert assigned by OpsGenie.\"\n    },\n    \"tinyId\": {\n      \"type\": \"string\",\n      \"description\": \"Short, human-readable identifier for the alert.\"\n    },\n    \"alias\": {\n      \"type\": \"string\",\n      \"maxLength\": 512,\n      \"description\": \"Client-defined identifier used for alert deduplication.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"maxLength\": 130,\n      \"description\": \"The alert message, limited\
  \ to 130 characters.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"maxLength\": 15000,\n      \"description\": \"Detailed description providing context about the alert.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"open\", \"closed\"],\n      \"description\": \"Current status of the alert.\"\n    },\n    \"acknowledged\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the alert has been acknowledged by a responder.\"\n    },\n    \"isSeen\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the alert has been viewed.\"\n    },\n    \"snoozed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the alert is currently snoozed.\"\n    },\n    \"snoozedUntil\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the snooze period ends.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\"\
  : \"string\"\n      },\n      \"maxItems\": 20,\n      \"description\": \"Tags attached to the alert for categorization.\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Number of times the alert has occurred (deduplication count).\"\n    },\n    \"lastOccurredAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time of the most recent occurrence.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the alert was first created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time of the last modification.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"Source of the alert, typically the integration or tool that created it.\"\n    },\n    \"owner\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"Username of the alert owner (assigned user).\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"enum\": [\"P1\", \"P2\", \"P3\", \"P4\", \"P5\"],\n      \"description\": \"Priority level from P1 (critical) to P5 (informational).\"\n    },\n    \"entity\": {\n      \"type\": \"string\",\n      \"maxLength\": 512,\n      \"description\": \"Entity field used to specify the domain of the alert.\"\n    },\n    \"responders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Responder\"\n      },\n      \"description\": \"Teams, users, escalations, and schedules responsible for the alert.\"\n    },\n    \"visibleTo\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Responder\"\n      },\n      \"description\": \"Teams and users who can see the alert without receiving notifications.\"\n    },\n    \"actions\": {\n      \"type\": \"array\",\n      \"items\"\
  : {\n        \"type\": \"string\"\n      },\n      \"maxItems\": 10,\n      \"description\": \"Custom actions available for the alert.\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Custom key-value pairs providing additional context.\"\n    },\n    \"integration\": {\n      \"$ref\": \"#/$defs/Integration\"\n    },\n    \"report\": {\n      \"$ref\": \"#/$defs/AlertReport\"\n    }\n  },\n  \"$defs\": {\n    \"Responder\": {\n      \"type\": \"object\",\n      \"required\": [\"type\"],\n      \"description\": \"A team, user, escalation, or schedule that responds to alerts.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the responder.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the responder (teams and schedules).\"\n        },\n  \
  \      \"username\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Username of the responder (users).\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"team\", \"user\", \"escalation\", \"schedule\"],\n          \"description\": \"Type of the responder entity.\"\n        }\n      }\n    },\n    \"Integration\": {\n      \"type\": \"object\",\n      \"description\": \"The integration that created the alert.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Integration ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Integration name.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Integration type.\"\n        }\n      }\n    },\n    \"AlertReport\": {\n      \"type\": \"object\",\n      \"description\": \"Report containing timing and\
  \ actor information for the alert lifecycle.\",\n      \"properties\": {\n        \"ackTime\": {\n          \"type\": \"integer\",\n          \"description\": \"Time in milliseconds from creation to acknowledgment.\"\n        },\n        \"closeTime\": {\n          \"type\": \"integer\",\n          \"description\": \"Time in milliseconds from creation to closure.\"\n        },\n        \"acknowledgedBy\": {\n          \"type\": \"string\",\n          \"description\": \"Username of the person who acknowledged the alert.\"\n        },\n        \"closedBy\": {\n          \"type\": \"string\",\n          \"description\": \"Username of the person who closed the alert.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/json-schema/opsgenie-alert-schema.json
tags:
- Alerts
- Incident Management
- Monitoring
- On-Call
- Operations
title: OpsGenie Alert
---
