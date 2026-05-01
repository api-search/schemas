---
description: CreateTableRequest schema from Amazon Glue API
layout: schema
name: CreateTableRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: TableInput
  type: object
- description: ''
  name: PartitionIndexes
  type: object
- description: ''
  name: TransactionId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-table-request-schema.json
slug: glue-create-table-request
source_filename: glue-create-table-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-table-request-schema.json\",\n  \"title\": \"CreateTableRequest\",\n  \"description\": \"CreateTableRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog in which to create the <code>Table</code>. If none is supplied, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The catalog database in which to create the new table. For Hive compatibility, this name is entirely lowercase.\"\
  \n        }\n      ]\n    },\n    \"TableInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TableInput\"\n        },\n        {\n          \"description\": \"The <code>TableInput</code> object that defines the metadata table to create in the catalog.\"\n        }\n      ]\n    },\n    \"PartitionIndexes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PartitionIndexList\"\n        },\n        {\n          \"description\": \"A list of partition indexes, <code>PartitionIndex</code> structures, to create in the table.\"\n        }\n      ]\n    },\n    \"TransactionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransactionIdString\"\n        },\n        {\n          \"description\": \"The ID of the transaction.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseName\",\n    \"TableInput\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-table-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateTableRequest
---
