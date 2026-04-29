---
description: DomainStatus schema from Amazon OpenSearch Service
layout: schema
name: DomainStatus
properties_list:
- description: ''
  name: DomainId
  type: string
- description: ''
  name: DomainName
  type: string
- description: ''
  name: ARN
  type: string
- description: ''
  name: Created
  type: boolean
- description: ''
  name: Deleted
  type: boolean
- description: ''
  name: Endpoint
  type: string
- description: ''
  name: EngineVersion
  type: string
provider_name: Amazon OpenSearch Service
provider_slug: amazon-opensearch-service
schema_file: json-schema/openapi-domain-status-schema.json
slug: openapi-domain-status
source_filename: openapi-domain-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch-service/refs/heads/main/json-schema/openapi-domain-status-schema.json\",\n  \"title\": \"DomainStatus\",\n  \"description\": \"DomainStatus schema from Amazon OpenSearch Service\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainId\": {\n      \"type\": \"string\"\n    },\n    \"DomainName\": {\n      \"type\": \"string\"\n    },\n    \"ARN\": {\n      \"type\": \"string\"\n    },\n    \"Created\": {\n      \"type\": \"boolean\"\n    },\n    \"Deleted\": {\n      \"type\": \"boolean\"\n    },\n    \"Endpoint\": {\n      \"type\": \"string\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch-service/refs/heads/main/json-schema/openapi-domain-status-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Full-Text Search
- Log Analytics
- OpenSearch
- Search
title: DomainStatus
---
