---
description: The record of the incident that's created when an incident occurs.
layout: schema
name: IncidentRecord
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: automationExecutions
  type: object
- description: ''
  name: chatChannel
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: dedupeString
  type: object
- description: ''
  name: impact
  type: object
- description: ''
  name: incidentRecordSource
  type: object
- description: ''
  name: lastModifiedBy
  type: object
- description: ''
  name: lastModifiedTime
  type: object
- description: ''
  name: notificationTargets
  type: object
- description: ''
  name: resolvedTime
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: summary
  type: object
- description: ''
  name: title
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-incident-record-schema.json
slug: incident-manager-incident-record
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-incident-record-schema.json\",\n  \"title\": \"IncidentRecord\",\n  \"description\": \"The record of the incident that's created when an incident occurs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the incident record.\"\n        }\n      ]\n    },\n    \"automationExecutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutomationExecutionSet\"\n        },\n        {\n          \"description\": \"The runbook, or automation document, that's run at the beginning of the incident.\"\n        }\n      ]\n    },\n    \"chatChannel\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/ChatChannel\"\n        },\n        {\n          \"description\": \"The chat channel used for collaboration during an incident.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that Incident Manager created the incident record.\"\n        }\n      ]\n    },\n    \"dedupeString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DedupeString\"\n        },\n        {\n          \"description\": \"The string Incident Manager uses to prevent duplicate incidents from being created by the same incident in the same account.\"\n        }\n      ]\n    },\n    \"impact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Impact\"\n        },\n        {\n          \"description\": \"The impact of the incident on customers and applications.\"\n\
  \        }\n      ]\n    },\n    \"incidentRecordSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentRecordSource\"\n        },\n        {\n          \"description\": \"Details about the action that started the incident.\"\n        }\n      ]\n    },\n    \"lastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"Who modified the incident most recently.\"\n        }\n      ]\n    },\n    \"lastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the incident was most recently modified.\"\n        }\n      ]\n    },\n    \"notificationTargets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationTargetSet\"\n        },\n        {\n          \"description\": \"The Amazon SNS targets that are\
  \ notified when updates are made to an incident.\"\n        }\n      ]\n    },\n    \"resolvedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the incident was resolved. This appears as a timeline event.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentRecordStatus\"\n        },\n        {\n          \"description\": \"The current status of the incident.\"\n        }\n      ]\n    },\n    \"summary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentSummary\"\n        },\n        {\n          \"description\": \"The summary of the incident. The summary is a brief synopsis of what occurred, what's currently happening, and context of the incident.\"\n        }\n      ]\n    },\n    \"title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentTitle\"\
  \n        },\n        {\n          \"description\": \"The title of the incident.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"creationTime\",\n    \"dedupeString\",\n    \"impact\",\n    \"incidentRecordSource\",\n    \"lastModifiedBy\",\n    \"lastModifiedTime\",\n    \"status\",\n    \"title\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-incident-record-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: IncidentRecord
---
