---
description: GetSchemaVersionInput schema from Amazon Glue API
layout: schema
name: GetSchemaVersionInput
properties_list:
- description: ''
  name: SchemaId
  type: object
- description: ''
  name: SchemaVersionId
  type: object
- description: ''
  name: SchemaVersionNumber
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-schema-version-input-schema.json
slug: glue-get-schema-version-input
source_filename: glue-get-schema-version-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-schema-version-input-schema.json\",\n  \"title\": \"GetSchemaVersionInput\",\n  \"description\": \"GetSchemaVersionInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaId\"\n        },\n        {\n          \"description\": \"<p>This is a wrapper structure to contain schema identity fields. The structure contains:</p> <ul> <li> <p>SchemaId$SchemaArn: The Amazon Resource Name (ARN) of the schema. Either <code>SchemaArn</code> or <code>SchemaName</code> and <code>RegistryName</code> has to be provided.</p> </li> <li> <p>SchemaId$SchemaName: The name of the schema. Either <code>SchemaArn</code> or <code>SchemaName</code> and <code>RegistryName</code> has to be provided.</p>\
  \ </li> </ul>\"\n        }\n      ]\n    },\n    \"SchemaVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionIdString\"\n        },\n        {\n          \"description\": \"The <code>SchemaVersionId</code> of the schema version. This field is required for fetching by schema ID. Either this or the <code>SchemaId</code> wrapper has to be provided.\"\n        }\n      ]\n    },\n    \"SchemaVersionNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionNumber\"\n        },\n        {\n          \"description\": \"The version number of the schema.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-schema-version-input-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetSchemaVersionInput
---
