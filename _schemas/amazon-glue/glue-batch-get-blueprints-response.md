---
description: BatchGetBlueprintsResponse schema from Amazon Glue API
layout: schema
name: BatchGetBlueprintsResponse
properties_list:
- description: ''
  name: Blueprints
  type: object
- description: ''
  name: MissingBlueprints
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-blueprints-response-schema.json
slug: glue-batch-get-blueprints-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-blueprints-response-schema.json\",\n  \"title\": \"BatchGetBlueprintsResponse\",\n  \"description\": \"BatchGetBlueprintsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Blueprints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Blueprints\"\n        },\n        {\n          \"description\": \"Returns a list of blueprint as a <code>Blueprints</code> object.\"\n        }\n      ]\n    },\n    \"MissingBlueprints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlueprintNames\"\n        },\n        {\n          \"description\": \"Returns a list of <code>BlueprintNames</code> that were not found.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-blueprints-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetBlueprintsResponse
---
