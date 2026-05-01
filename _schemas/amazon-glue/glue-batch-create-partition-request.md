---
description: BatchCreatePartitionRequest schema from Amazon Glue API
layout: schema
name: BatchCreatePartitionRequest
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
  name: PartitionInputList
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-create-partition-request-schema.json
slug: glue-batch-create-partition-request
source_filename: glue-batch-create-partition-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-create-partition-request-schema.json\",\n  \"title\": \"BatchCreatePartitionRequest\",\n  \"description\": \"BatchCreatePartitionRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the catalog in which the partition is to be created. Currently, this should be the Amazon Web Services account ID.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the metadata database in which the partition is to be created.\"\n        }\n      ]\n    },\n\
  \    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the metadata table in which the partition is to be created.\"\n        }\n      ]\n    },\n    \"PartitionInputList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PartitionInputList\"\n        },\n        {\n          \"description\": \"A list of <code>PartitionInput</code> structures that define the partitions to be created.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseName\",\n    \"TableName\",\n    \"PartitionInputList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-create-partition-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchCreatePartitionRequest
---
