---
description: Connection schema from Oracle Integration Developer API.
layout: schema
name: Connection
properties_list:
- description: Connection identifier.
  name: id
  type: string
- description: Connection display name.
  name: name
  type: string
- description: Connection description.
  name: description
  type: string
- description: Connection status.
  name: status
  type: string
- description: Type of adapter used by the connection.
  name: adapterType
  type: string
- description: Percentage of connection configuration completion.
  name: percentageComplete
  type: integer
- description: Whether the connection is locked.
  name: lockedFlag
  type: boolean
- description: Last test status.
  name: testStatus
  type: string
- description: User who last updated the connection.
  name: lastUpdatedBy
  type: string
- description: Last update timestamp.
  name: lastUpdated
  type: string
provider_name: Oracle Integration
provider_slug: oracle-integration
schema_file: json-schema/developer-api-connection-schema.json
slug: developer-api-connection
source_filename: developer-api-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/json-schema/developer-api-connection-schema.json\",\n  \"title\": \"Connection\",\n  \"description\": \"Connection schema from Oracle Integration Developer API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"string\", \"description\": \"Connection identifier.\"},\n    \"name\": {\"type\": \"string\", \"description\": \"Connection display name.\"},\n    \"description\": {\"type\": \"string\", \"description\": \"Connection description.\"},\n    \"status\": {\"type\": \"string\", \"description\": \"Connection status.\", \"enum\": [\"CONFIGURED\", \"DRAFT\", \"ERROR\"]},\n    \"adapterType\": {\"type\": \"string\", \"description\": \"Type of adapter used by the connection.\"},\n    \"percentageComplete\": {\"type\": \"integer\", \"description\": \"Percentage of connection configuration completion.\"\
  },\n    \"lockedFlag\": {\"type\": \"boolean\", \"description\": \"Whether the connection is locked.\"},\n    \"testStatus\": {\"type\": \"string\", \"description\": \"Last test status.\"},\n    \"lastUpdatedBy\": {\"type\": \"string\", \"description\": \"User who last updated the connection.\"},\n    \"lastUpdated\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"Last update timestamp.\"}\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/json-schema/developer-api-connection-schema.json
tags:
- API Management
- Automation
- B2B Integration
- Cloud Integration
- Enterprise Integration
- Integration
- iPaaS
- Process Automation
title: Connection
---
