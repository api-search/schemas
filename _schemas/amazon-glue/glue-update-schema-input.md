---
description: UpdateSchemaInput schema from Amazon Glue API
layout: schema
name: UpdateSchemaInput
properties_list:
- description: ''
  name: SchemaId
  type: object
- description: ''
  name: SchemaVersionNumber
  type: object
- description: ''
  name: Compatibility
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-schema-input-schema.json
slug: glue-update-schema-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-schema-input-schema.json\",\n  \"title\": \"UpdateSchemaInput\",\n  \"description\": \"UpdateSchemaInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaId\"\n        },\n        {\n          \"description\": \"<p>This is a wrapper structure to contain schema identity fields. The structure contains:</p> <ul> <li> <p>SchemaId$SchemaArn: The Amazon Resource Name (ARN) of the schema. One of <code>SchemaArn</code> or <code>SchemaName</code> has to be provided.</p> </li> <li> <p>SchemaId$SchemaName: The name of the schema. One of <code>SchemaArn</code> or <code>SchemaName</code> has to be provided.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"SchemaVersionNumber\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionNumber\"\n        },\n        {\n          \"description\": \"Version number required for check pointing. One of <code>VersionNumber</code> or <code>Compatibility</code> has to be provided.\"\n        }\n      ]\n    },\n    \"Compatibility\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Compatibility\"\n        },\n        {\n          \"description\": \"The new compatibility setting for the schema.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"The new description for the schema.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SchemaId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-schema-input-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateSchemaInput
---
