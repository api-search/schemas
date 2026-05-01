---
description: DomainStatus schema
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
  name: Processing
  type: boolean
- description: ''
  name: RequiresIndexDocuments
  type: boolean
- description: ''
  name: SearchInstanceCount
  type: integer
- description: ''
  name: SearchInstanceType
  type: string
- description: ''
  name: DocService
  type: object
- description: ''
  name: SearchService
  type: object
provider_name: Amazon CloudSearch
provider_slug: amazon-cloudsearch
schema_file: json-schema/cloudsearch-domain-status-schema.json
slug: cloudsearch-domain-status
source_filename: cloudsearch-domain-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudsearch/refs/heads/main/json-schema/cloudsearch-domain-status-schema.json\",\n  \"title\": \"DomainStatus\",\n  \"description\": \"DomainStatus schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainId\": {\n      \"type\": \"string\"\n    },\n    \"DomainName\": {\n      \"type\": \"string\"\n    },\n    \"ARN\": {\n      \"type\": \"string\"\n    },\n    \"Created\": {\n      \"type\": \"boolean\"\n    },\n    \"Deleted\": {\n      \"type\": \"boolean\"\n    },\n    \"Processing\": {\n      \"type\": \"boolean\"\n    },\n    \"RequiresIndexDocuments\": {\n      \"type\": \"boolean\"\n    },\n    \"SearchInstanceCount\": {\n      \"type\": \"integer\"\n    },\n    \"SearchInstanceType\": {\n      \"type\": \"string\"\n    },\n    \"DocService\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Endpoint\"\
  : {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"SearchService\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Endpoint\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudsearch/refs/heads/main/json-schema/cloudsearch-domain-status-schema.json
tags:
- CloudSearch
- Search
- Full-Text Search
- Managed
title: DomainStatus
---
