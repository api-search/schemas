---
description: RegisterSchemaVersionResponse schema from Amazon Glue API
layout: schema
name: RegisterSchemaVersionResponse
properties_list:
- description: ''
  name: SchemaVersionId
  type: object
- description: ''
  name: VersionNumber
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-register-schema-version-response-schema.json
slug: glue-register-schema-version-response
source_filename: glue-register-schema-version-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-register-schema-version-response-schema.json\",\n  \"title\": \"RegisterSchemaVersionResponse\",\n  \"description\": \"RegisterSchemaVersionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionIdString\"\n        },\n        {\n          \"description\": \"The unique ID that represents the version of this schema.\"\n        }\n      ]\n    },\n    \"VersionNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionLongNumber\"\n        },\n        {\n          \"description\": \"The version of this schema (for sync flow only, in case this is the first version).\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionStatus\"\n        },\n        {\n          \"description\": \"The status of the schema version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-register-schema-version-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: RegisterSchemaVersionResponse
---
