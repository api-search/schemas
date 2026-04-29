---
description: PutSchemaVersionMetadataInput schema from Amazon Glue API
layout: schema
name: PutSchemaVersionMetadataInput
properties_list:
- description: ''
  name: SchemaId
  type: object
- description: ''
  name: SchemaVersionNumber
  type: object
- description: ''
  name: SchemaVersionId
  type: object
- description: ''
  name: MetadataKeyValue
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-put-schema-version-metadata-input-schema.json
slug: glue-put-schema-version-metadata-input
source_filename: glue-put-schema-version-metadata-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-put-schema-version-metadata-input-schema.json\",\n  \"title\": \"PutSchemaVersionMetadataInput\",\n  \"description\": \"PutSchemaVersionMetadataInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaId\"\n        },\n        {\n          \"description\": \"The unique ID for the schema.\"\n        }\n      ]\n    },\n    \"SchemaVersionNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionNumber\"\n        },\n        {\n          \"description\": \"The version number of the schema.\"\n        }\n      ]\n    },\n    \"SchemaVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionIdString\"\
  \n        },\n        {\n          \"description\": \"The unique version ID of the schema version.\"\n        }\n      ]\n    },\n    \"MetadataKeyValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetadataKeyValuePair\"\n        },\n        {\n          \"description\": \"The metadata key's corresponding value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MetadataKeyValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-put-schema-version-metadata-input-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: PutSchemaVersionMetadataInput
---
