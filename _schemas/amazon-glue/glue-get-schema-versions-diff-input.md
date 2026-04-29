---
description: GetSchemaVersionsDiffInput schema from Amazon Glue API
layout: schema
name: GetSchemaVersionsDiffInput
properties_list:
- description: ''
  name: SchemaId
  type: object
- description: ''
  name: FirstSchemaVersionNumber
  type: object
- description: ''
  name: SecondSchemaVersionNumber
  type: object
- description: ''
  name: SchemaDiffType
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-schema-versions-diff-input-schema.json
slug: glue-get-schema-versions-diff-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-schema-versions-diff-input-schema.json\",\n  \"title\": \"GetSchemaVersionsDiffInput\",\n  \"description\": \"GetSchemaVersionsDiffInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaId\"\n        },\n        {\n          \"description\": \"<p>This is a wrapper structure to contain schema identity fields. The structure contains:</p> <ul> <li> <p>SchemaId$SchemaArn: The Amazon Resource Name (ARN) of the schema. One of <code>SchemaArn</code> or <code>SchemaName</code> has to be provided.</p> </li> <li> <p>SchemaId$SchemaName: The name of the schema. One of <code>SchemaArn</code> or <code>SchemaName</code> has to be provided.</p> </li> </ul>\"\n        }\n      ]\n    },\n\
  \    \"FirstSchemaVersionNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionNumber\"\n        },\n        {\n          \"description\": \"The first of the two schema versions to be compared.\"\n        }\n      ]\n    },\n    \"SecondSchemaVersionNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionNumber\"\n        },\n        {\n          \"description\": \"The second of the two schema versions to be compared.\"\n        }\n      ]\n    },\n    \"SchemaDiffType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaDiffType\"\n        },\n        {\n          \"description\": \"Refers to <code>SYNTAX_DIFF</code>, which is the currently supported diff type.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SchemaId\",\n    \"FirstSchemaVersionNumber\",\n    \"SecondSchemaVersionNumber\",\n    \"SchemaDiffType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-schema-versions-diff-input-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetSchemaVersionsDiffInput
---
