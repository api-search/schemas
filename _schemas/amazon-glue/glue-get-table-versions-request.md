---
description: GetTableVersionsRequest schema from Amazon Glue API
layout: schema
name: GetTableVersionsRequest
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
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-table-versions-request-schema.json
slug: glue-get-table-versions-request
source_filename: glue-get-table-versions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-table-versions-request-schema.json\",\n  \"title\": \"GetTableVersionsRequest\",\n  \"description\": \"GetTableVersionsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog where the tables reside. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The database in the catalog in which the table resides. For Hive compatibility, this name is entirely lowercase.\"\
  \n        }\n      ]\n    },\n    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the table. For Hive compatibility, this name is entirely lowercase.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if this is not the first call.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogGetterPageSize\"\n        },\n        {\n          \"description\": \"The maximum number of table versions to return in one response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseName\",\n    \"TableName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-table-versions-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetTableVersionsRequest
---
