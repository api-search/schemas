---
description: Connection information for dataset input files stored in a database.
layout: schema
name: DatabaseInputDefinition
properties_list:
- description: ''
  name: GlueConnectionName
  type: object
- description: ''
  name: DatabaseTableName
  type: object
- description: ''
  name: TempDirectory
  type: object
- description: ''
  name: QueryString
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-database-input-definition-schema.json
slug: glue-databrew-database-input-definition
source_filename: glue-databrew-database-input-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-database-input-definition-schema.json\",\n  \"title\": \"DatabaseInputDefinition\",\n  \"description\": \"Connection information for dataset input files stored in a database.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GlueConnectionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueConnectionName\"\n        },\n        {\n          \"description\": \"The Glue Connection that stores the connection information for the target database.\"\n        }\n      ]\n    },\n    \"DatabaseTableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseTableName\"\n        },\n        {\n          \"description\": \"The table within the target database.\"\n        }\n      ]\n    },\n    \"TempDirectory\": {\n  \
  \    \"$ref\": \"#/components/schemas/S3Location\"\n    },\n    \"QueryString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryString\"\n        },\n        {\n          \"description\": \"Custom SQL to run against the provided Glue connection. This SQL will be used as the input for DataBrew projects and jobs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GlueConnectionName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-database-input-definition-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: DatabaseInputDefinition
---
