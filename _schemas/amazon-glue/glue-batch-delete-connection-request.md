---
description: BatchDeleteConnectionRequest schema from Amazon Glue API
layout: schema
name: BatchDeleteConnectionRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: ConnectionNameList
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-delete-connection-request-schema.json
slug: glue-batch-delete-connection-request
source_filename: glue-batch-delete-connection-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-delete-connection-request-schema.json\",\n  \"title\": \"BatchDeleteConnectionRequest\",\n  \"description\": \"BatchDeleteConnectionRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog in which the connections reside. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"ConnectionNameList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeleteConnectionNameList\"\n        },\n        {\n          \"description\": \"A list of names of the connections to delete.\"\n        }\n      ]\n\
  \    }\n  },\n  \"required\": [\n    \"ConnectionNameList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-delete-connection-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchDeleteConnectionRequest
---
