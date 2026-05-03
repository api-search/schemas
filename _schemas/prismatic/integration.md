---
description: An integration defines a workflow connecting your product to a third-party service. Integrations are built in the designer and deployed as instances to customers.
layout: schema
name: Prismatic Integration
properties_list:
- description: Unique identifier for the integration
  name: id
  type: string
- description: Name of the integration
  name: name
  type: string
- description: Description of the integration and what it does
  name: description
  type: string
- description: Category for organizing integrations
  name: category
  type: string
- description: Labels applied to the integration for categorization
  name: labels
  type: array
- description: Detailed overview of the integration displayed in the marketplace
  name: overview
  type: string
- description: Current version number of the integration
  name: versionNumber
  type: integer
- description: Whether the current version is available for deployment
  name: versionIsAvailable
  type: boolean
- description: Whether the integration is built using code-native (CNI) approach
  name: isCodeNative
  type: boolean
- description: List of flows within the integration
  name: flows
  type: array
- description: Deployed instances of the integration
  name: instances
  type: array
- description: Visibility setting for the integration marketplace
  name: marketplaceConfiguration
  type: string
- description: Timestamp when the integration was created
  name: createdAt
  type: string
- description: Timestamp when the integration was last updated
  name: updatedAt
  type: string
provider_name: Prismatic
provider_slug: prismatic
schema_file: json-schema/integration.json
slug: integration
source_filename: integration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/integration.json\",\n  \"title\": \"Prismatic Integration\",\n  \"description\": \"An integration defines a workflow connecting your product to a third-party service. Integrations are built in the designer and deployed as instances to customers.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the integration\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the integration\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the integration and what it does\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category for organizing integrations\"\n    },\n \
  \   \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the integration for categorization\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"overview\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed overview of the integration displayed in the marketplace\"\n    },\n    \"versionNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Current version number of the integration\"\n    },\n    \"versionIsAvailable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the current version is available for deployment\"\n    },\n    \"isCodeNative\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the integration is built using code-native (CNI) approach\"\n    },\n    \"flows\": {\n      \"type\": \"array\",\n      \"description\": \"List of flows within the integration\",\n      \"items\": {\n        \"$ref\": \"flow.json\"\n      }\n    },\n    \"instances\": {\n   \
  \   \"type\": \"array\",\n      \"description\": \"Deployed instances of the integration\",\n      \"items\": {\n        \"$ref\": \"instance.json\"\n      }\n    },\n    \"marketplaceConfiguration\": {\n      \"type\": \"string\",\n      \"enum\": [\"AVAILABLE\", \"HIDDEN\"],\n      \"description\": \"Visibility setting for the integration marketplace\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the integration was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the integration was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/integration.json
tags:
- Embedded iPaaS
- Integrations
- Workflows
title: Prismatic Integration
---
