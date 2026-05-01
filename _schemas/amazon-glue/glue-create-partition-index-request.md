---
description: CreatePartitionIndexRequest schema from Amazon Glue API
layout: schema
name: CreatePartitionIndexRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: TableName
  type: object
- description: ''
  name: PartitionIndex
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-partition-index-request-schema.json
slug: glue-create-partition-index-request
source_filename: glue-create-partition-index-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-partition-index-request-schema.json\",\n  \"title\": \"CreatePartitionIndexRequest\",\n  \"description\": \"CreatePartitionIndexRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The catalog ID where the table resides.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Specifies the name of a database in which you want to create a partition index.\"\n        }\n      ]\n    },\n    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\
  \n        },\n        {\n          \"description\": \"Specifies the name of a table in which you want to create a partition index.\"\n        }\n      ]\n    },\n    \"PartitionIndex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PartitionIndex\"\n        },\n        {\n          \"description\": \"Specifies a <code>PartitionIndex</code> structure to create a partition index in an existing table.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseName\",\n    \"TableName\",\n    \"PartitionIndex\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-partition-index-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreatePartitionIndexRequest
---
