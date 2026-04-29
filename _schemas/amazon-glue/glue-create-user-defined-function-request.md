---
description: CreateUserDefinedFunctionRequest schema from Amazon Glue API
layout: schema
name: CreateUserDefinedFunctionRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: FunctionInput
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-user-defined-function-request-schema.json
slug: glue-create-user-defined-function-request
source_filename: glue-create-user-defined-function-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-user-defined-function-request-schema.json\",\n  \"title\": \"CreateUserDefinedFunctionRequest\",\n  \"description\": \"CreateUserDefinedFunctionRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog in which to create the function. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the catalog database in which to create the function.\"\n      \
  \  }\n      ]\n    },\n    \"FunctionInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserDefinedFunctionInput\"\n        },\n        {\n          \"description\": \"A <code>FunctionInput</code> object that defines the function to create in the Data Catalog.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseName\",\n    \"FunctionInput\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-user-defined-function-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateUserDefinedFunctionRequest
---
