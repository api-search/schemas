---
description: Represents an incident in the OpsGenie platform. Incidents are higher-level events that may affect services and require coordinated response across teams.
layout: schema
name: OpsGenie Incident
properties_list:
- description: Unique identifier of the incident.
  name: id
  type: string
- description: Short, human-readable identifier.
  name: tinyId
  type: string
- description: The incident message, limited to 130 characters.
  name: message
  type: string
- description: Detailed description of the incident.
  name: description
  type: string
- description: Current status of the incident.
  name: status
  type: string
- description: Tags for categorization.
  name: tags
  type: array
- description: Priority level from P1 (critical) to P5 (informational).
  name: priority
  type: string
- description: Date and time when the incident was created.
  name: createdAt
  type: string
- description: Date and time of the last modification.
  name: updatedAt
  type: string
- description: The owner team of the incident.
  name: ownerTeam
  type: string
- description: Teams assigned to respond to the incident.
  name: responders
  type: array
- description: IDs of services impacted by the incident.
  name: impactedServices
  type: array
- description: Custom key-value pairs providing additional context.
  name: details
  type: object
- description: Whether stakeholders are notified about the incident.
  name: notifyStakeholders
  type: boolean
- description: ''
  name: statusPageEntry
  type: object
provider_name: OpsGenie
provider_slug: opsgenie
schema_file: json-schema/opsgenie-incident-schema.json
slug: opsgenie-incident
source_filename: opsgenie-incident-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api-evangelist.com/opsgenie/incident.json\",\n  \"title\": \"OpsGenie Incident\",\n  \"description\": \"Represents an incident in the OpsGenie platform. Incidents are higher-level events that may affect services and require coordinated response across teams.\",\n  \"type\": \"object\",\n  \"required\": [\"message\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the incident.\"\n    },\n    \"tinyId\": {\n      \"type\": \"string\",\n      \"description\": \"Short, human-readable identifier.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"maxLength\": 130,\n      \"description\": \"The incident message, limited to 130 characters.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"maxLength\": 10000,\n      \"description\": \"Detailed description of the incident.\"\n    },\n\
  \    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"open\", \"resolved\", \"closed\"],\n      \"description\": \"Current status of the incident.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"maxItems\": 20,\n      \"description\": \"Tags for categorization.\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"enum\": [\"P1\", \"P2\", \"P3\", \"P4\", \"P5\"],\n      \"description\": \"Priority level from P1 (critical) to P5 (informational).\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the incident was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time of the last modification.\"\n    },\n    \"ownerTeam\": {\n      \"type\": \"string\",\n      \"description\": \"The owner team of the incident.\"\
  \n    },\n    \"responders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/IncidentResponder\"\n      },\n      \"description\": \"Teams assigned to respond to the incident.\"\n    },\n    \"impactedServices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IDs of services impacted by the incident.\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Custom key-value pairs providing additional context.\"\n    },\n    \"notifyStakeholders\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether stakeholders are notified about the incident.\"\n    },\n    \"statusPageEntry\": {\n      \"$ref\": \"#/$defs/StatusPageEntry\"\n    }\n  },\n  \"$defs\": {\n    \"IncidentResponder\": {\n      \"type\": \"object\",\n      \"description\": \"A team assigned to respond to the incident.\"\
  ,\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Team ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Team name.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"team\"],\n          \"description\": \"Type of responder, currently only team is supported for incidents.\"\n        }\n      }\n    },\n    \"StatusPageEntry\": {\n      \"type\": \"object\",\n      \"description\": \"A status page entry associated with the incident.\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Title of the status page entry.\"\n        },\n        \"detail\": {\n          \"type\": \"string\",\n          \"description\": \"Detail message for the status page.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/json-schema/opsgenie-incident-schema.json
tags:
- Alerts
- Incident Management
- Monitoring
- On-Call
- Operations
title: OpsGenie Incident
---
