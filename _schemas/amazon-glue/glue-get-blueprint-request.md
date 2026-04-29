---
description: GetBlueprintRequest schema from Amazon Glue API
layout: schema
name: GetBlueprintRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: IncludeBlueprint
  type: object
- description: ''
  name: IncludeParameterSpec
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-blueprint-request-schema.json
slug: glue-get-blueprint-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-blueprint-request-schema.json\",\n  \"title\": \"GetBlueprintRequest\",\n  \"description\": \"GetBlueprintRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the blueprint.\"\n        }\n      ]\n    },\n    \"IncludeBlueprint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Specifies whether or not to include the blueprint in the response.\"\n        }\n      ]\n    },\n    \"IncludeParameterSpec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n  \
  \      },\n        {\n          \"description\": \"Specifies whether or not to include the parameter specification.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-blueprint-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetBlueprintRequest
---
