---
description: GetColumnStatisticsForPartitionRequest schema from Amazon Glue API
layout: schema
name: GetColumnStatisticsForPartitionRequest
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
  name: PartitionValues
  type: object
- description: ''
  name: ColumnNames
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-column-statistics-for-partition-request-schema.json
slug: glue-get-column-statistics-for-partition-request
source_filename: glue-get-column-statistics-for-partition-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-column-statistics-for-partition-request-schema.json\",\n  \"title\": \"GetColumnStatisticsForPartitionRequest\",\n  \"description\": \"GetColumnStatisticsForPartitionRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog where the partitions in question reside. If none is supplied, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the catalog database where the partitions\
  \ reside.\"\n        }\n      ]\n    },\n    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the partitions' table.\"\n        }\n      ]\n    },\n    \"PartitionValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueStringList\"\n        },\n        {\n          \"description\": \"A list of partition values identifying the partition.\"\n        }\n      ]\n    },\n    \"ColumnNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetColumnNamesList\"\n        },\n        {\n          \"description\": \"A list of the column names.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseName\",\n    \"TableName\",\n    \"PartitionValues\",\n    \"ColumnNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-column-statistics-for-partition-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetColumnStatisticsForPartitionRequest
---
