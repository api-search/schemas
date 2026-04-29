---
description: GetSchemaByDefinitionInput schema from Amazon Glue API
layout: schema
name: GetSchemaByDefinitionInput
properties_list:
- description: ''
  name: SchemaId
  type: object
- description: ''
  name: SchemaDefinition
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-schema-by-definition-input-schema.json
slug: glue-get-schema-by-definition-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-schema-by-definition-input-schema.json\",\n  \"title\": \"GetSchemaByDefinitionInput\",\n  \"description\": \"GetSchemaByDefinitionInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaId\"\n        },\n        {\n          \"description\": \"<p>This is a wrapper structure to contain schema identity fields. The structure contains:</p> <ul> <li> <p>SchemaId$SchemaArn: The Amazon Resource Name (ARN) of the schema. One of <code>SchemaArn</code> or <code>SchemaName</code> has to be provided.</p> </li> <li> <p>SchemaId$SchemaName: The name of the schema. One of <code>SchemaArn</code> or <code>SchemaName</code> has to be provided.</p> </li> </ul>\"\n        }\n      ]\n    },\n\
  \    \"SchemaDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaDefinitionString\"\n        },\n        {\n          \"description\": \"The definition of the schema for which schema details are required.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SchemaId\",\n    \"SchemaDefinition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-schema-by-definition-input-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetSchemaByDefinitionInput
---
