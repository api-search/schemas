---
description: BatchGetBlueprintsRequest schema from Amazon Glue API
layout: schema
name: BatchGetBlueprintsRequest
properties_list:
- description: ''
  name: Names
  type: object
- description: ''
  name: IncludeBlueprint
  type: object
- description: ''
  name: IncludeParameterSpec
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-blueprints-request-schema.json
slug: glue-batch-get-blueprints-request
source_filename: glue-batch-get-blueprints-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-blueprints-request-schema.json\",\n  \"title\": \"BatchGetBlueprintsRequest\",\n  \"description\": \"BatchGetBlueprintsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Names\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetBlueprintNames\"\n        },\n        {\n          \"description\": \"A list of blueprint names.\"\n        }\n      ]\n    },\n    \"IncludeBlueprint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Specifies whether or not to include the blueprint in the response.\"\n        }\n      ]\n    },\n    \"IncludeParameterSpec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\
  \n        },\n        {\n          \"description\": \"Specifies whether or not to include the parameters, as a JSON string, for the blueprint in the response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Names\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-blueprints-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetBlueprintsRequest
---
