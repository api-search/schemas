---
description: Schema for a Sandbox Banking (Glyue) integration definition. An integration is a wrapper for composable logic that connects external banking systems through service requests, field mappings, value mappings, and validation rules.
layout: schema
name: Sandbox Banking Integration
properties_list:
- description: Unique identifier for the integration.
  name: id
  type: string
- description: Human-readable name of the integration (e.g., 'Loan Booking to Fiserv Spectrum').
  name: name
  type: string
- description: Description of what this integration does and which systems it connects.
  name: description
  type: string
- description: Current status of the integration.
  name: status
  type: string
- description: Type of integration pattern.
  name: integrationType
  type: string
- description: The system that sends data into this integration.
  name: sourceSystem
  type: object
- description: The system that receives data from this integration.
  name: targetSystem
  type: object
- description: Ordered list of service request operations that make up this integration.
  name: serviceRequests
  type: array
- description: Field mapping definitions that transform data between source and target formats.
  name: fieldMappings
  type: array
- description: Validation rules that enforce input/response compliance.
  name: validationRules
  type: array
- description: Whether run history audit logging is enabled for this integration.
  name: auditEnabled
  type: boolean
- description: Timestamp when the integration was created.
  name: createdAt
  type: string
- description: Timestamp when the integration was last modified.
  name: updatedAt
  type: string
provider_name: Sandbox Banking
provider_slug: sandbox-banking
schema_file: json-schema/sandbox-banking-integration-schema.json
slug: sandbox-banking-integration
source_filename: sandbox-banking-integration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"sandbox-banking-integration-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Sandbox Banking Integration\",\n  \"description\": \"Schema for a Sandbox Banking (Glyue) integration definition. An integration is a wrapper for composable logic that connects external banking systems through service requests, field mappings, value mappings, and validation rules.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the integration.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the integration (e.g., 'Loan Booking to Fiserv Spectrum').\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what this integration does and which systems it connects.\"\n    },\n    \"status\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Current status of the integration.\",\n      \"enum\": [\"active\", \"inactive\", \"draft\", \"testing\", \"deprecated\"]\n    },\n    \"integrationType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of integration pattern.\",\n      \"enum\": [\"web_service_api\", \"batch_etl\", \"file_transfer\", \"event_pubsub\", \"webhook\"]\n    },\n    \"sourceSystem\": {\n      \"type\": \"object\",\n      \"description\": \"The system that sends data into this integration.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Source system name (e.g., nCino, Salesforce CRM, Client Portal).\"\n        },\n        \"adapterType\": {\n          \"type\": \"string\",\n          \"description\": \"Adapter type used to connect to the source system.\"\n        }\n      }\n    },\n    \"targetSystem\": {\n      \"type\": \"object\",\n      \"description\": \"The system that receives data\
  \ from this integration.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Target system name (e.g., Fiserv Signature, Jack Henry Symitar, FIS Modern Banking).\"\n        },\n        \"adapterType\": {\n          \"type\": \"string\",\n          \"description\": \"Adapter type used to connect to the target system.\"\n        }\n      }\n    },\n    \"serviceRequests\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered list of service request operations that make up this integration.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Service request name.\"\n          },\n          \"adapter\": {\n            \"type\": \"string\",\n            \"description\": \"Adapter used for this service request.\"\n          },\n          \"operation\": {\n            \"type\": \"string\",\n            \"\
  description\": \"Operation being performed (e.g., createLoan, getAccount, postTransaction).\"\n          },\n          \"callForEach\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this service request iterates over a list of inputs.\"\n          }\n        }\n      }\n    },\n    \"fieldMappings\": {\n      \"type\": \"array\",\n      \"description\": \"Field mapping definitions that transform data between source and target formats.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"sourceField\": {\n            \"type\": \"string\",\n            \"description\": \"Source field path or expression.\"\n          },\n          \"targetField\": {\n            \"type\": \"string\",\n            \"description\": \"Target field path.\"\n          },\n          \"transform\": {\n            \"type\": \"string\",\n            \"description\": \"Optional transformation formula or function.\"\n          }\n        }\n  \
  \    }\n    },\n    \"validationRules\": {\n      \"type\": \"array\",\n      \"description\": \"Validation rules that enforce input/response compliance.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"condition\": {\n            \"type\": \"string\",\n            \"description\": \"Boolean expression that must be true for the integration to proceed.\"\n          },\n          \"errorMessage\": {\n            \"type\": \"string\",\n            \"description\": \"Error message returned if validation fails.\"\n          }\n        }\n      }\n    },\n    \"auditEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether run history audit logging is enabled for this integration.\",\n      \"default\": true\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the integration was\
  \ created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the integration was last modified.\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sandbox-banking/refs/heads/main/json-schema/sandbox-banking-integration-schema.json
tags:
- API Integration
- Banking
- Core Banking
- Credit Unions
- Financial Services
- Fintech
- Integration Platform
- iPaaS
- Open Banking
title: Sandbox Banking Integration
---
