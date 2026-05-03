---
description: A connection to a third-party business platform via the Rutter Unified API
layout: schema
name: Rutter Connection
properties_list:
- description: Unique identifier for the connection
  name: id
  type: string
- description: The connected platform identifier (e.g., quickbooks, shopify, amazon)
  name: platform
  type: string
- description: Current connection status
  name: status
  type: string
- description: Timestamp when the connection was created
  name: created_at
  type: string
- description: Timestamp when the connection was last updated
  name: updated_at
  type: string
provider_name: Rutter
provider_slug: rutter
schema_file: json-schema/rutter-connection-schema.json
slug: rutter-connection
source_filename: rutter-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://api-evangelist.github.io/rutter/json-schema/rutter-connection-schema.json\",\n  \"title\": \"Rutter Connection\",\n  \"description\": \"A connection to a third-party business platform via the Rutter Unified API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the connection\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"The connected platform identifier (e.g., quickbooks, shopify, amazon)\",\n      \"examples\": [\"quickbooks\", \"xero\", \"shopify\", \"amazon\", \"woocommerce\", \"netsuite\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"inactive\", \"error\"],\n      \"description\": \"Current connection status\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Timestamp when the connection was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the connection was last updated\"\n    }\n  },\n  \"required\": [\"id\", \"platform\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rutter/refs/heads/main/json-schema/rutter-connection-schema.json
tags:
- Accounting
- B2B
- Commerce
- Financial Data
- Payments
- Unified API
title: Rutter Connection
---
