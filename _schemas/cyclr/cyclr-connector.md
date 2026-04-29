---
description: A Cyclr connector represents a pre-built integration with a third-party application or service. Connectors define the available methods, authentication, and data mappings for interacting with external APIs.
layout: schema
name: Cyclr Connector
properties_list:
- description: Unique connector identifier
  name: Id
  type: integer
- description: Connector name
  name: Name
  type: string
- description: Connector description
  name: Description
  type: string
- description: Connector status
  name: Status
  type: string
- description: Connector version
  name: Version
  type: string
- description: URL to the connector icon
  name: Icon
  type: string
- description: Authentication type used by the connector
  name: AuthType
  type: string
provider_name: Cyclr
provider_slug: cyclr
schema_file: json-schema/cyclr-connector.json
slug: cyclr-connector
source_filename: cyclr-connector.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/json-schema/cyclr-connector.json\",\n  \"title\": \"Cyclr Connector\",\n  \"description\": \"A Cyclr connector represents a pre-built integration with a third-party application or service. Connectors define the available methods, authentication, and data mappings for interacting with external APIs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique connector identifier\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Connector name\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Connector description\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Connector status\"\n    },\n    \"Version\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Connector version\"\n    },\n    \"Icon\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the connector icon\"\n    },\n    \"AuthType\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication type used by the connector\",\n      \"enum\": [\"OAuth2\", \"OAuth1\", \"ApiKey\", \"Basic\", \"None\"]\n    }\n  },\n  \"required\": [\"Id\", \"Name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/json-schema/cyclr-connector.json
tags:
- Connectors
- Custom Connectors
- Data Synchronization
- Embedded iPaaS
- Embedded SaaS Integration
- Embedded UI
- Integration Platform
- Integrations
- Marketplace
- OAuth 2.0
- REST API
- SaaS
- Templates
- Webhooks
- White Label
- Workflows
title: Cyclr Connector
---
