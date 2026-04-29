---
description: A Cyclr account represents a tenant or customer environment within the Cyclr iPaaS platform. Each account contains its own installed connectors, cycles, and configuration.
layout: schema
name: Cyclr Account
properties_list:
- description: Unique account identifier
  name: Id
  type: string
- description: Account name
  name: Name
  type: string
- description: Account description
  name: Description
  type: string
- description: External API identifier for the account
  name: ApiId
  type: string
- description: Number of audiences in the account
  name: AudienceCount
  type: integer
- description: When the account was created
  name: CreatedDate
  type: string
- description: Connectors installed in the account
  name: Connectors
  type: array
provider_name: Cyclr
provider_slug: cyclr
schema_file: json-schema/cyclr-account.json
slug: cyclr-account
source_filename: cyclr-account.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/json-schema/cyclr-account.json\",\n  \"title\": \"Cyclr Account\",\n  \"description\": \"A Cyclr account represents a tenant or customer environment within the Cyclr iPaaS platform. Each account contains its own installed connectors, cycles, and configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique account identifier\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Account name\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Account description\"\n    },\n    \"ApiId\": {\n      \"type\": \"string\",\n      \"description\": \"External API identifier for the account\"\n    },\n    \"AudienceCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of\
  \ audiences in the account\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the account was created\"\n    },\n    \"Connectors\": {\n      \"type\": \"array\",\n      \"description\": \"Connectors installed in the account\",\n      \"items\": {\n        \"$ref\": \"cyclr-installed-connector.json\"\n      }\n    }\n  },\n  \"required\": [\"Id\", \"Name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/json-schema/cyclr-account.json
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
title: Cyclr Account
---
