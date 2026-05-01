---
description: An entitlement representing a granular access right from an onboarded target application. Entitlements are aggregated into a centralized catalog by Identity Governance for review, certification, and compliance purposes.
layout: schema
name: ForgeRock Entitlement
properties_list:
- description: Unique identifier for the entitlement
  name: _id
  type: string
- description: Entitlement name
  name: name
  type: string
- description: Human-readable description of the entitlement
  name: description
  type: string
- description: Name of the application that owns this entitlement
  name: applicationName
  type: string
- description: Identifier of the owning application
  name: applicationId
  type: string
- description: Type of entitlement
  name: type
  type: string
- description: User identifier of the entitlement owner
  name: owner
  type: string
- description: Risk classification for the entitlement
  name: riskLevel
  type: string
- description: Business glossary metadata for the entitlement
  name: glossary
  type: object
- description: Number of users currently assigned this entitlement
  name: assignedUsers
  type: integer
provider_name: ForgeRock
provider_slug: forgerock
schema_file: json-schema/forgerock-entitlement-schema.json
slug: forgerock-entitlement
source_filename: forgerock-entitlement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.forgerock.com/entitlement\",\n  \"title\": \"ForgeRock Entitlement\",\n  \"description\": \"An entitlement representing a granular access right from an onboarded target application. Entitlements are aggregated into a centralized catalog by Identity Governance for review, certification, and compliance purposes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the entitlement\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Entitlement name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the entitlement\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the application that owns this entitlement\"\n    },\n    \"applicationId\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Identifier of the owning application\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of entitlement\",\n      \"enum\": [\"group\", \"permission\", \"role\", \"privilege\", \"license\"]\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"User identifier of the entitlement owner\"\n    },\n    \"riskLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Risk classification for the entitlement\",\n      \"enum\": [\"low\", \"medium\", \"high\", \"critical\"]\n    },\n    \"glossary\": {\n      \"type\": \"object\",\n      \"description\": \"Business glossary metadata for the entitlement\",\n      \"properties\": {\n        \"displayName\": {\n          \"type\": \"string\"\n        },\n        \"requestable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether users can request this entitlement\"\n        },\n        \"approvalRequired\"\
  : {\n          \"type\": \"boolean\",\n          \"description\": \"Whether approval is required to grant this entitlement\"\n        }\n      }\n    },\n    \"assignedUsers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of users currently assigned this entitlement\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"name\", \"applicationName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/json-schema/forgerock-entitlement-schema.json
tags:
- Access Management
- Authentication
- Authorization
- Identity Governance
- Identity Management
- OAuth
- OpenID Connect
title: ForgeRock Entitlement
---
