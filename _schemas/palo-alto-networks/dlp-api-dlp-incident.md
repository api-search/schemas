---
description: DLPIncident schema from Palo Alto Networks Enterprise DLP API
layout: schema
name: DLPIncident
properties_list:
- description: Unique incident identifier.
  name: incident_id
  type: string
- description: Current incident status.
  name: status
  type: string
- description: Incident severity level.
  name: severity
  type: string
- description: Name of the data pattern that triggered the incident.
  name: data_pattern_name
  type: string
- description: Identifier of the data pattern that triggered the incident.
  name: data_pattern_id
  type: string
- description: Number of data pattern matches in the content.
  name: match_count
  type: integer
- description: Channel where the data exposure was detected.
  name: channel
  type: string
- description: Email address or username of the user involved.
  name: user
  type: string
- description: Timestamp when the incident was detected.
  name: timestamp
  type: string
- description: Application associated with the incident.
  name: application
  type: string
- description: Name of the file containing sensitive data.
  name: file_name
  type: string
- description: MIME type of the file.
  name: file_type
  type: string
- description: Size of the file in bytes.
  name: file_size
  type: integer
- description: Direction of data movement.
  name: direction
  type: string
- description: Automated action taken on the incident.
  name: action_taken
  type: string
- description: Comments added by the reviewing analyst.
  name: reviewer_comments
  type: string
- description: Email address of the analyst who reviewed the incident.
  name: reviewed_by
  type: string
- description: Timestamp when the incident was last reviewed.
  name: reviewed_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/dlp-api-dlp-incident-schema.json
slug: dlp-api-dlp-incident
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DLPIncident\",\n  \"description\": \"DLPIncident schema from Palo Alto Networks Enterprise DLP API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/dlp-api-dlp-incident-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"incident_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique incident identifier.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"open\",\n        \"in_review\",\n        \"resolved\",\n        \"dismissed\"\n      ],\n      \"description\": \"Current incident status.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\",\n        \"informational\"\n      ],\n      \"description\": \"Incident severity level.\"\n    },\n    \"data_pattern_name\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Name of the data pattern that triggered the incident.\"\n    },\n    \"data_pattern_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the data pattern that triggered the incident.\"\n    },\n    \"match_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of data pattern matches in the content.\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"web\",\n        \"ssl\",\n        \"saas\",\n        \"email\",\n        \"endpoint\"\n      ],\n      \"description\": \"Channel where the data exposure was detected.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"Email address or username of the user involved.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the incident was detected.\"\n    },\n    \"application\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Application associated with the incident.\"\n    },\n    \"file_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the file containing sensitive data.\"\n    },\n    \"file_type\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the file.\"\n    },\n    \"file_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the file in bytes.\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"upload\",\n        \"download\",\n        \"internal\"\n      ],\n      \"description\": \"Direction of data movement.\"\n    },\n    \"action_taken\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"alert\",\n        \"block\",\n        \"quarantine\",\n        \"encrypt\"\n      ],\n      \"description\": \"Automated action taken on the incident.\"\n    },\n    \"reviewer_comments\": {\n      \"type\": \"string\",\n      \"description\": \"Comments added\
  \ by the reviewing analyst.\"\n    },\n    \"reviewed_by\": {\n      \"type\": \"string\",\n      \"description\": \"Email address of the analyst who reviewed the incident.\"\n    },\n    \"reviewed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the incident was last reviewed.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/dlp-api-dlp-incident-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DLPIncident
---
