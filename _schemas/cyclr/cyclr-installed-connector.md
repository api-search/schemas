---
description: An installed connector is an instance of a Cyclr connector that has been deployed into a specific account. It holds account-level authentication credentials and configuration for the connector.
layout: schema
name: Cyclr Installed Connector
properties_list:
- description: Installed connector identifier
  name: Id
  type: integer
- description: Installed connector name
  name: Name
  type: string
- description: Installed connector description
  name: Description
  type: string
- description: Reference to the base connector
  name: ConnectorId
  type: integer
- description: Whether the connector has been authenticated
  name: Authenticated
  type: boolean
- description: Installation status
  name: Status
  type: string
provider_name: Cyclr
provider_slug: cyclr
schema_file: json-schema/cyclr-installed-connector.json
slug: cyclr-installed-connector
source_filename: cyclr-installed-connector.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/json-schema/cyclr-installed-connector.json\",\n  \"title\": \"Cyclr Installed Connector\",\n  \"description\": \"An installed connector is an instance of a Cyclr connector that has been deployed into a specific account. It holds account-level authentication credentials and configuration for the connector.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"integer\",\n      \"description\": \"Installed connector identifier\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Installed connector name\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Installed connector description\"\n    },\n    \"ConnectorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Reference to the base connector\"\n    },\n    \"Authenticated\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the connector has been authenticated\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Installation status\"\n    }\n  },\n  \"required\": [\"Id\", \"ConnectorId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/json-schema/cyclr-installed-connector.json
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
title: Cyclr Installed Connector
---
