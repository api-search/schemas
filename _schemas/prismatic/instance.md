---
description: An instance is a deployment of an integration to a specific customer, with customer-specific configuration values.
layout: schema
name: Prismatic Instance
properties_list:
- description: Unique identifier for the instance
  name: id
  type: string
- description: Name of the instance
  name: name
  type: string
- description: Description of the instance
  name: description
  type: string
- description: Whether the instance is currently enabled and running
  name: enabled
  type: boolean
- description: Whether the instance has been deployed
  name: deployed
  type: boolean
- description: Whether the instance needs to be redeployed after configuration changes
  name: needsDeploy
  type: boolean
- description: The customer this instance is deployed to
  name: customer
  type: object
- description: The integration this instance is based on
  name: integration
  type: object
- description: Configuration variables specific to this instance
  name: configVariables
  type: array
- description: Flow-level configuration for this instance
  name: flowConfigs
  type: array
- description: Labels applied to the instance
  name: labels
  type: array
- description: Timestamp of the last deployment
  name: lastDeployedAt
  type: string
- description: Timestamp when the instance was created
  name: createdAt
  type: string
- description: Timestamp when the instance was last updated
  name: updatedAt
  type: string
provider_name: Prismatic
provider_slug: prismatic
schema_file: json-schema/instance.json
slug: instance
source_filename: instance.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/instance.json\",\n  \"title\": \"Prismatic Instance\",\n  \"description\": \"An instance is a deployment of an integration to a specific customer, with customer-specific configuration values.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the instance\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the instance\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the instance\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the instance is currently enabled and running\"\n    },\n    \"deployed\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the instance has been deployed\"\n    },\n    \"needsDeploy\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the instance needs to be redeployed after configuration changes\"\n    },\n    \"customer\": {\n      \"$ref\": \"customer.json\",\n      \"description\": \"The customer this instance is deployed to\"\n    },\n    \"integration\": {\n      \"$ref\": \"integration.json\",\n      \"description\": \"The integration this instance is based on\"\n    },\n    \"configVariables\": {\n      \"type\": \"array\",\n      \"description\": \"Configuration variables specific to this instance\",\n      \"items\": {\n        \"$ref\": \"config-variable.json\"\n      }\n    },\n    \"flowConfigs\": {\n      \"type\": \"array\",\n      \"description\": \"Flow-level configuration for this instance\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"flow\": {\n            \"$ref\": \"flow.json\"\n          },\n          \"apiEndpointUrl\"\
  : {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"Webhook endpoint URL for the flow\"\n          }\n        }\n      }\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the instance\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"lastDeployedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last deployment\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the instance was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the instance was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/instance.json
tags:
- Embedded iPaaS
- Integrations
- Workflows
title: Prismatic Instance
---
