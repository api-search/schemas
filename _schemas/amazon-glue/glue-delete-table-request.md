---
description: DeleteTableRequest schema from Amazon Glue API
layout: schema
name: DeleteTableRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: TransactionId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-table-request-schema.json
slug: glue-delete-table-request
source_filename: glue-delete-table-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-table-request-schema.json\",\n  \"title\": \"DeleteTableRequest\",\n  \"description\": \"DeleteTableRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog where the table resides. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the catalog database in which the table resides. For Hive compatibility, this name is entirely lowercase.\"\n      \
  \  }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the table to be deleted. For Hive compatibility, this name is entirely lowercase.\"\n        }\n      ]\n    },\n    \"TransactionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransactionIdString\"\n        },\n        {\n          \"description\": \"The transaction ID at which to delete the table contents.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseName\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-table-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteTableRequest
---
