---
description: A data lake namespace
layout: schema
name: DataLakeNamespace
properties_list:
- description: The instance identifier
  name: instanceId
  type: string
- description: The namespace name
  name: name
  type: string
- description: The namespace description
  name: description
  type: string
- description: ''
  name: createdTime
  type: string
- description: ''
  name: lastModifiedTime
  type: string
provider_name: Amazon Supply Chain
provider_slug: amazon-supply-chain
schema_file: json-schema/amazon-supply-chain-data-lake-namespace-schema.json
slug: amazon-supply-chain-data-lake-namespace
source_filename: amazon-supply-chain-data-lake-namespace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/json-schema/amazon-supply-chain-data-lake-namespace-schema.json\",\n  \"title\": \"DataLakeNamespace\",\n  \"description\": \"A data lake namespace\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The instance identifier\",\n      \"example\": \"inst-abc12345\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace name\",\n      \"example\": \"asc\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace description\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/json-schema/amazon-supply-chain-data-lake-namespace-schema.json
tags:
- ERP Integration
- Logistics
- Machine Learning
- Supply Chain
title: DataLakeNamespace
---
