---
description: EmailDLPIncident schema from Palo Alto Networks Email DLP API
layout: schema
name: EmailDLPIncident
properties_list:
- description: Unique incident identifier.
  name: id
  type: string
- description: Email address of the message sender.
  name: sender
  type: string
- description: Email message subject line.
  name: subject
  type: string
- description: Current status or verdict for the email message.
  name: status
  type: string
- description: Incident severity based on data pattern sensitivity.
  name: severity
  type: string
- description: Data patterns that matched in the email content.
  name: data_patterns
  type: array
- description: Total number of data pattern matches across all patterns.
  name: match_count
  type: integer
- description: Timestamp when the incident was detected.
  name: timestamp
  type: string
- description: Whether the email contained attachments.
  name: has_attachments
  type: boolean
- description: Number of attachments in the email.
  name: attachment_count
  type: integer
- description: Direction of the email message.
  name: direction
  type: string
- description: Automated action taken on the message.
  name: action_taken
  type: string
- description: Email address of the analyst who reviewed the incident.
  name: reviewed_by
  type: string
- description: Timestamp when the incident was last reviewed.
  name: reviewed_at
  type: string
- description: Comment added during verdict review.
  name: comment
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/email-dlp-api-email-dlp-incident-schema.json
slug: email-dlp-api-email-dlp-incident
source_filename: email-dlp-api-email-dlp-incident-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailDLPIncident\",\n  \"description\": \"EmailDLPIncident schema from Palo Alto Networks Email DLP API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/email-dlp-api-email-dlp-incident-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique incident identifier.\"\n    },\n    \"sender\": {\n      \"type\": \"string\",\n      \"description\": \"Email address of the message sender.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Email message subject line.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"allowed\",\n        \"blocked\",\n        \"quarantined\"\n      ],\n      \"description\": \"Current status or verdict for the email message.\"\n    },\n\
  \    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\",\n        \"informational\"\n      ],\n      \"description\": \"Incident severity based on data pattern sensitivity.\"\n    },\n    \"data_patterns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"category\": {\n            \"type\": \"string\"\n          },\n          \"match_count\": {\n            \"type\": \"integer\"\n          }\n        }\n      },\n      \"description\": \"Data patterns that matched in the email content.\"\n    },\n    \"match_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of data pattern matches across all patterns.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the incident was detected.\"\n    },\n    \"has_attachments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email contained attachments.\"\n    },\n    \"attachment_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of attachments in the email.\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"inbound\",\n        \"outbound\",\n        \"internal\"\n      ],\n      \"description\": \"Direction of the email message.\"\n    },\n    \"action_taken\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"alert\",\n        \"block\",\n        \"quarantine\"\n      ],\n      \"description\": \"Automated action taken on the message.\"\n    },\n    \"reviewed_by\": {\n      \"type\": \"string\",\n      \"description\": \"Email address of the analyst who reviewed the incident.\"\n    },\n    \"reviewed_at\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the incident was last reviewed.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comment added during verdict review.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/email-dlp-api-email-dlp-incident-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: EmailDLPIncident
---
