---
description: BatchDeleteTableVersionRequest schema from Amazon Glue API
layout: schema
name: BatchDeleteTableVersionRequest
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
  name: VersionIds
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-delete-table-version-request-schema.json
slug: glue-batch-delete-table-version-request
source_filename: glue-batch-delete-table-version-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-delete-table-version-request-schema.json\",\n  \"title\": \"BatchDeleteTableVersionRequest\",\n  \"description\": \"BatchDeleteTableVersionRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog where the tables reside. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The database in the catalog in which the table resides. For Hive compatibility, this name\
  \ is entirely lowercase.\"\n        }\n      ]\n    },\n    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the table. For Hive compatibility, this name is entirely lowercase.\"\n        }\n      ]\n    },\n    \"VersionIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchDeleteTableVersionList\"\n        },\n        {\n          \"description\": \"A list of the IDs of versions to be deleted. A <code>VersionId</code> is a string representation of an integer. Each version is incremented by 1.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseName\",\n    \"TableName\",\n    \"VersionIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-delete-table-version-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchDeleteTableVersionRequest
---
