---
description: A data lake dataset
layout: schema
name: DataLakeDataset
properties_list:
- description: The instance identifier
  name: instanceId
  type: string
- description: The namespace containing the dataset
  name: namespace
  type: string
- description: The dataset name
  name: name
  type: string
- description: The dataset description
  name: description
  type: string
- description: The dataset schema
  name: schema
  type: object
- description: The partition specification
  name: partitionSpec
  type: object
- description: ''
  name: createdTime
  type: string
- description: ''
  name: lastModifiedTime
  type: string
provider_name: Amazon Supply Chain
provider_slug: amazon-supply-chain
schema_file: json-schema/amazon-supply-chain-data-lake-dataset-schema.json
slug: amazon-supply-chain-data-lake-dataset
source_filename: amazon-supply-chain-data-lake-dataset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/json-schema/amazon-supply-chain-data-lake-dataset-schema.json\",\n  \"title\": \"DataLakeDataset\",\n  \"description\": \"A data lake dataset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The instance identifier\",\n      \"example\": \"inst-abc12345\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace containing the dataset\",\n      \"example\": \"asc\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The dataset name\",\n      \"example\": \"product\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The dataset description\"\n    },\n    \"schema\": {\n      \"type\": \"object\",\n      \"description\": \"The dataset\
  \ schema\"\n    },\n    \"partitionSpec\": {\n      \"type\": \"object\",\n      \"description\": \"The partition specification\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/json-schema/amazon-supply-chain-data-lake-dataset-schema.json
tags:
- ERP Integration
- Logistics
- Machine Learning
- Supply Chain
title: DataLakeDataset
---
