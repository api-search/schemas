---
description: DeleteSchemaVersionsResponse schema from Amazon Glue API
layout: schema
name: DeleteSchemaVersionsResponse
properties_list:
- description: ''
  name: SchemaVersionErrors
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-schema-versions-response-schema.json
slug: glue-delete-schema-versions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-schema-versions-response-schema.json\",\n  \"title\": \"DeleteSchemaVersionsResponse\",\n  \"description\": \"DeleteSchemaVersionsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaVersionErrors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionErrorList\"\n        },\n        {\n          \"description\": \"A list of <code>SchemaVersionErrorItem</code> objects, each containing an error and schema version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-schema-versions-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteSchemaVersionsResponse
---
