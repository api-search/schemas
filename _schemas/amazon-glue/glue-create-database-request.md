---
description: CreateDatabaseRequest schema from Amazon Glue API
layout: schema
name: CreateDatabaseRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: DatabaseInput
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-database-request-schema.json
slug: glue-create-database-request
source_filename: glue-create-database-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-database-request-schema.json\",\n  \"title\": \"CreateDatabaseRequest\",\n  \"description\": \"CreateDatabaseRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog in which to create the database. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"DatabaseInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseInput\"\n        },\n        {\n          \"description\": \"The metadata for the database.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"The tags you assign to the database.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseInput\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-database-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateDatabaseRequest
---
