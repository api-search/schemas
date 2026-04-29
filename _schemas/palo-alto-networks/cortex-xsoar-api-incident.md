---
description: A Cortex XSOAR incident representing a security event under investigation.
layout: schema
name: Incident
properties_list:
- description: Unique incident identifier.
  name: id
  type: string
- description: Incident name or title.
  name: name
  type: string
- description: Incident type (maps to an incident type definition).
  name: type
  type: string
- description: 'Incident status code: 0 (Pending), 1 (Active), 2 (Done), 3 (Archive).'
  name: status
  type: integer
- description: 'Severity level: 0 (Unknown), 1 (Informational), 2 (Low), 3 (Medium), 4 (High), 5 (Critical).'
  name: severity
  type: integer
- description: Username of the analyst assigned to this incident.
  name: owner
  type: string
- description: Incident creation timestamp.
  name: created
  type: string
- description: Last modification timestamp.
  name: modified
  type: string
- description: Timestamp when the security event occurred.
  name: occurred
  type: string
- description: Incident closure timestamp.
  name: closed
  type: string
- description: Reason for closing the incident.
  name: closeReason
  type: string
- description: Notes added when closing the incident.
  name: closeNotes
  type: string
- description: Key-value label pairs attached to the incident.
  name: labels
  type: array
- description: Incident details or description.
  name: details
  type: string
- description: Associated investigation ID.
  name: investigationId
  type: string
- description: Playbook assigned to this incident.
  name: playbookId
  type: string
- description: Integration instance that created this incident.
  name: sourceInstance
  type: string
- description: Integration brand that created this incident.
  name: sourceBrand
  type: string
- description: Raw JSON payload from the originating event.
  name: rawJson
  type: string
- description: Custom field values specific to the incident type.
  name: CustomFields
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsoar-api-incident-schema.json
slug: cortex-xsoar-api-incident
source_filename: cortex-xsoar-api-incident-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Incident\",\n  \"description\": \"A Cortex XSOAR incident representing a security event under investigation.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-incident-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique incident identifier.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Incident name or title.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Incident type (maps to an incident type definition).\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"Incident status code: 0 (Pending), 1 (Active), 2 (Done), 3 (Archive).\",\n      \"enum\": [\n        0,\n        1,\n        2,\n        3\n   \
  \   ]\n    },\n    \"severity\": {\n      \"type\": \"integer\",\n      \"description\": \"Severity level: 0 (Unknown), 1 (Informational), 2 (Low), 3 (Medium), 4 (High), 5 (Critical).\",\n      \"enum\": [\n        0,\n        1,\n        2,\n        3,\n        4,\n        5\n      ]\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the analyst assigned to this incident.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Incident creation timestamp.\",\n      \"readOnly\": true\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp.\",\n      \"readOnly\": true\n    },\n    \"occurred\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the security event occurred.\"\n    },\n    \"closed\": {\n      \"type\": \"string\",\n      \"\
  format\": \"date-time\",\n      \"description\": \"Incident closure timestamp.\"\n    },\n    \"closeReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for closing the incident.\"\n    },\n    \"closeNotes\": {\n      \"type\": \"string\",\n      \"description\": \"Notes added when closing the incident.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"Key-value label pairs attached to the incident.\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Incident details or description.\"\n    },\n    \"investigationId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated investigation ID.\",\n      \"readOnly\": true\n    },\n    \"playbookId\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Playbook assigned to this incident.\"\n    },\n    \"sourceInstance\": {\n      \"type\": \"string\",\n      \"description\": \"Integration instance that created this incident.\"\n    },\n    \"sourceBrand\": {\n      \"type\": \"string\",\n      \"description\": \"Integration brand that created this incident.\"\n    },\n    \"rawJson\": {\n      \"type\": \"string\",\n      \"description\": \"Raw JSON payload from the originating event.\"\n    },\n    \"CustomFields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom field values specific to the incident type.\",\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-incident-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Incident
---
