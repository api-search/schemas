---
description: Metadata about an API proxy in Apigee. API proxies act as facades for backend services, providing security, rate limiting, transformations, and other capabilities.
layout: schema
name: Apigee API Proxy
properties_list:
- description: Output only. Name of the API proxy.
  name: name
  type: string
- description: Output only. List of revisions defined for the API proxy.
  name: revision
  type: array
- description: Output only. The ID of the most recently created revision.
  name: latestRevisionId
  type: string
- description: ''
  name: metaData
  type: object
- description: User-defined labels for organizing API proxies.
  name: labels
  type: object
- description: Output only. Whether this proxy is read-only.
  name: readOnly
  type: boolean
- description: Type of the API proxy.
  name: apiProxyType
  type: string
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-api-proxy-schema.json
slug: apigee-api-proxy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/apigee/apigee-api-proxy-schema.json\",\n  \"title\": \"Apigee API Proxy\",\n  \"description\": \"Metadata about an API proxy in Apigee. API proxies act as facades for backend services, providing security, rate limiting, transformations, and other capabilities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Name of the API proxy.\",\n      \"readOnly\": true\n    },\n    \"revision\": {\n      \"type\": \"array\",\n      \"description\": \"Output only. List of revisions defined for the API proxy.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"latestRevisionId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The ID of the most recently created revision.\",\n      \"readOnly\": true\n    },\n    \"metaData\": {\n\
  \      \"$ref\": \"#/$defs/EntityMetadata\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"User-defined labels for organizing API proxies.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"readOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Output only. Whether this proxy is read-only.\",\n      \"readOnly\": true\n    },\n    \"apiProxyType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the API proxy.\",\n      \"enum\": [\"API_PROXY_TYPE_UNSPECIFIED\", \"PROGRAMMABLE\", \"CONFIGURABLE\"]\n    }\n  },\n  \"$defs\": {\n    \"EntityMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata common to Apigee entities.\",\n      \"properties\": {\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"description\": \"Time the entity was created in milliseconds since epoch.\"\n        },\n        \"lastModifiedAt\": {\n          \"type\": \"\
  string\",\n          \"description\": \"Time the entity was last modified in milliseconds since epoch.\"\n        },\n        \"subType\": {\n          \"type\": \"string\",\n          \"description\": \"Subtype of the entity.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/json-schema/apigee-api-proxy-schema.json
tags:
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Hybrid
- Integrations
- Microservices
- Monetization
title: Apigee API Proxy
---
