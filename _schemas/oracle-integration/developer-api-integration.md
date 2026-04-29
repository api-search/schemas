---
description: Integration schema from Oracle Integration Developer API.
layout: schema
name: Integration
properties_list:
- description: Integration identifier.
  name: id
  type: string
- description: Integration code.
  name: code
  type: string
- description: Integration version.
  name: version
  type: string
- description: Integration display name.
  name: name
  type: string
- description: Integration description.
  name: description
  type: string
- description: Integration status.
  name: status
  type: string
- description: Integration pattern type.
  name: pattern
  type: string
- description: Integration style.
  name: style
  type: string
- description: Whether the integration is locked.
  name: lockedFlag
  type: boolean
- description: User who last updated.
  name: lastUpdatedBy
  type: string
- description: Last update timestamp.
  name: lastUpdated
  type: string
- description: Package name the integration belongs to.
  name: packageName
  type: string
provider_name: Oracle Integration
provider_slug: oracle-integration
schema_file: json-schema/developer-api-integration-schema.json
slug: developer-api-integration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/json-schema/developer-api-integration-schema.json\",\n  \"title\": \"Integration\",\n  \"description\": \"Integration schema from Oracle Integration Developer API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"string\", \"description\": \"Integration identifier.\"},\n    \"code\": {\"type\": \"string\", \"description\": \"Integration code.\"},\n    \"version\": {\"type\": \"string\", \"description\": \"Integration version.\"},\n    \"name\": {\"type\": \"string\", \"description\": \"Integration display name.\"},\n    \"description\": {\"type\": \"string\", \"description\": \"Integration description.\"},\n    \"status\": {\"type\": \"string\", \"description\": \"Integration status.\", \"enum\": [\"CONFIGURED\", \"ACTIVATED\", \"DRAFT\"]},\n    \"pattern\": {\"type\": \"string\", \"description\"\
  : \"Integration pattern type.\"},\n    \"style\": {\"type\": \"string\", \"description\": \"Integration style.\"},\n    \"lockedFlag\": {\"type\": \"boolean\", \"description\": \"Whether the integration is locked.\"},\n    \"lastUpdatedBy\": {\"type\": \"string\", \"description\": \"User who last updated.\"},\n    \"lastUpdated\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"Last update timestamp.\"},\n    \"packageName\": {\"type\": \"string\", \"description\": \"Package name the integration belongs to.\"}\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/json-schema/developer-api-integration-schema.json
tags:
- API Management
- Automation
- B2B Integration
- Cloud Integration
- Enterprise Integration
- Integration
- iPaaS
- Process Automation
title: Integration
---
