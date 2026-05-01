---
description: CheckSchemaVersionValidityResponse schema from Amazon Glue API
layout: schema
name: CheckSchemaVersionValidityResponse
properties_list:
- description: ''
  name: Valid
  type: object
- description: ''
  name: Error
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-check-schema-version-validity-response-schema.json
slug: glue-check-schema-version-validity-response
source_filename: glue-check-schema-version-validity-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-check-schema-version-validity-response-schema.json\",\n  \"title\": \"CheckSchemaVersionValidityResponse\",\n  \"description\": \"CheckSchemaVersionValidityResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Valid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IsVersionValid\"\n        },\n        {\n          \"description\": \"Return true, if the schema is valid and false otherwise.\"\n        }\n      ]\n    },\n    \"Error\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaValidationError\"\n        },\n        {\n          \"description\": \"A validation failure error message.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-check-schema-version-validity-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CheckSchemaVersionValidityResponse
---
