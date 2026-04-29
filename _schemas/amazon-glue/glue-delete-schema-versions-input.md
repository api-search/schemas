---
description: DeleteSchemaVersionsInput schema from Amazon Glue API
layout: schema
name: DeleteSchemaVersionsInput
properties_list:
- description: ''
  name: SchemaId
  type: object
- description: ''
  name: Versions
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-schema-versions-input-schema.json
slug: glue-delete-schema-versions-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-schema-versions-input-schema.json\",\n  \"title\": \"DeleteSchemaVersionsInput\",\n  \"description\": \"DeleteSchemaVersionsInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaId\"\n        },\n        {\n          \"description\": \"This is a wrapper structure that may contain the schema name and Amazon Resource Name (ARN).\"\n        }\n      ]\n    },\n    \"Versions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionsString\"\n        },\n        {\n          \"description\": \"<p>A version range may be supplied which may be of the format:</p> <ul> <li> <p>a single version number, 5</p> </li> <li> <p>a range, 5-8 : deletes versions\
  \ 5, 6, 7, 8</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SchemaId\",\n    \"Versions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-schema-versions-input-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteSchemaVersionsInput
---
