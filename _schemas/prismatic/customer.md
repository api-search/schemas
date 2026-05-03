---
description: A customer represents a company or organization that uses your product and has integrations deployed to them in Prismatic.
layout: schema
name: Prismatic Customer
properties_list:
- description: Unique identifier for the customer
  name: id
  type: string
- description: Name of the customer organization
  name: name
  type: string
- description: Optional description of the customer
  name: description
  type: string
- description: External identifier used to map the customer to your own system
  name: externalId
  type: string
- description: URL of the customer avatar image
  name: avatarUrl
  type: string
- description: Labels applied to the customer for categorization
  name: labels
  type: array
- description: Whether the customer is allowed to use the embedded designer
  name: allowEmbeddedDesigner
  type: boolean
- description: Timestamp when the customer was created
  name: createdAt
  type: string
- description: Timestamp when the customer was last updated
  name: updatedAt
  type: string
provider_name: Prismatic
provider_slug: prismatic
schema_file: json-schema/customer.json
slug: customer
source_filename: customer.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/customer.json\",\n  \"title\": \"Prismatic Customer\",\n  \"description\": \"A customer represents a company or organization that uses your product and has integrations deployed to them in Prismatic.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the customer\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the customer organization\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the customer\"\n    },\n    \"externalId\": {\n      \"type\": \"string\",\n      \"description\": \"External identifier used to map the customer to your own system\"\n    },\n    \"avatarUrl\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the customer avatar image\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the customer for categorization\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"allowEmbeddedDesigner\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the customer is allowed to use the embedded designer\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the customer was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the customer was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/customer.json
tags:
- Embedded iPaaS
- Integrations
- Workflows
title: Prismatic Customer
---
