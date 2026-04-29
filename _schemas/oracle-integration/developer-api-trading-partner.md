---
description: TradingPartner schema from Oracle Integration Developer API.
layout: schema
name: TradingPartner
properties_list:
- description: Trading partner identifier.
  name: id
  type: string
- description: Trading partner name.
  name: name
  type: string
- description: Trading partner description.
  name: description
  type: string
- description: Partner status.
  name: status
  type: string
- description: Contact person name.
  name: contactName
  type: string
- description: Contact email address.
  name: contactEmail
  type: string
provider_name: Oracle Integration
provider_slug: oracle-integration
schema_file: json-schema/developer-api-trading-partner-schema.json
slug: developer-api-trading-partner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/json-schema/developer-api-trading-partner-schema.json\",\n  \"title\": \"TradingPartner\",\n  \"description\": \"TradingPartner schema from Oracle Integration Developer API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"string\", \"description\": \"Trading partner identifier.\"},\n    \"name\": {\"type\": \"string\", \"description\": \"Trading partner name.\"},\n    \"description\": {\"type\": \"string\", \"description\": \"Trading partner description.\"},\n    \"status\": {\"type\": \"string\", \"description\": \"Partner status.\", \"enum\": [\"ACTIVE\", \"INACTIVE\"]},\n    \"contactName\": {\"type\": \"string\", \"description\": \"Contact person name.\"},\n    \"contactEmail\": {\"type\": \"string\", \"format\": \"email\", \"description\": \"Contact email address.\"}\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/json-schema/developer-api-trading-partner-schema.json
tags:
- API Management
- Automation
- B2B Integration
- Cloud Integration
- Enterprise Integration
- Integration
- iPaaS
- Process Automation
title: TradingPartner
---
