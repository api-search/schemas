---
description: An API endpoint discovered and tracked by the Salt Security API Protection Platform.
layout: schema
name: Salt Security API Endpoint
properties_list:
- description: Unique identifier for the discovered API endpoint
  name: id
  type: string
- description: HTTP method
  name: method
  type: string
- description: API endpoint path
  name: path
  type: string
- description: API host/domain
  name: host
  type: string
- description: Parent API identifier this endpoint belongs to
  name: api_id
  type: string
- description: Name of the parent API
  name: api_name
  type: string
- description: Status of the endpoint
  name: status
  type: string
- description: Whether this endpoint exists in OpenAPI/Swagger documentation
  name: is_documented
  type: boolean
- description: Whether this is a shadow endpoint (undiscovered, not in OAS docs)
  name: is_shadow
  type: boolean
- description: Whether this is a zombie endpoint (deprecated but still accessible)
  name: is_zombie
  type: boolean
- description: Sensitive data fields found in this endpoint
  name: sensitive_data
  type: array
- description: Risk score for this endpoint (0-100)
  name: risk_score
  type: number
- description: Identified vulnerabilities for this endpoint
  name: vulnerabilities
  type: array
- description: Whether authentication is required for this endpoint
  name: authentication_required
  type: boolean
- description: Timestamp when endpoint was first discovered
  name: first_seen
  type: string
- description: Timestamp of most recent traffic
  name: last_seen
  type: string
provider_name: Salt Security
provider_slug: salt-security
schema_file: json-schema/salt-security-api-endpoint-schema.json
slug: salt-security-api-endpoint
source_filename: salt-security-api-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/salt-security/json-schema/salt-security-api-endpoint-schema.json\",\n  \"title\": \"Salt Security API Endpoint\",\n  \"description\": \"An API endpoint discovered and tracked by the Salt Security API Protection Platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the discovered API endpoint\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP method\",\n      \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\", \"OPTIONS\", \"HEAD\"]\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"API endpoint path\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"API host/domain\"\n    },\n    \"api_id\": {\n      \"type\": \"string\",\n      \"description\": \"Parent API identifier\
  \ this endpoint belongs to\"\n    },\n    \"api_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the parent API\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the endpoint\",\n      \"enum\": [\"active\", \"deprecated\", \"shadow\", \"zombie\", \"undocumented\"]\n    },\n    \"is_documented\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this endpoint exists in OpenAPI/Swagger documentation\"\n    },\n    \"is_shadow\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a shadow endpoint (undiscovered, not in OAS docs)\"\n    },\n    \"is_zombie\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a zombie endpoint (deprecated but still accessible)\"\n    },\n    \"sensitive_data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n \
  \           \"description\": \"Type of sensitive data (PII, PCI, PHI, credentials)\"\n          },\n          \"parameter\": {\n            \"type\": \"string\",\n            \"description\": \"Parameter name containing sensitive data\"\n          },\n          \"location\": {\n            \"type\": \"string\",\n            \"enum\": [\"request\", \"response\"],\n            \"description\": \"Where sensitive data appears\"\n          }\n        }\n      },\n      \"description\": \"Sensitive data fields found in this endpoint\"\n    },\n    \"risk_score\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Risk score for this endpoint (0-100)\"\n    },\n    \"vulnerabilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          },\n        \
  \  \"severity\": {\n            \"type\": \"string\",\n            \"enum\": [\"critical\", \"high\", \"medium\", \"low\", \"informational\"]\n          },\n          \"description\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"Identified vulnerabilities for this endpoint\"\n    },\n    \"authentication_required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether authentication is required for this endpoint\"\n    },\n    \"first_seen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when endpoint was first discovered\"\n    },\n    \"last_seen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of most recent traffic\"\n    }\n  },\n  \"required\": [\"id\", \"method\", \"path\", \"host\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salt-security/refs/heads/main/json-schema/salt-security-api-endpoint-schema.json
tags:
- API Security
- AI
- API Discovery
- Posture Governance
- Threat Protection
- Security
title: Salt Security API Endpoint
---
