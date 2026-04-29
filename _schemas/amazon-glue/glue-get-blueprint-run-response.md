---
description: GetBlueprintRunResponse schema from Amazon Glue API
layout: schema
name: GetBlueprintRunResponse
properties_list:
- description: ''
  name: BlueprintRun
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-blueprint-run-response-schema.json
slug: glue-get-blueprint-run-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-blueprint-run-response-schema.json\",\n  \"title\": \"GetBlueprintRunResponse\",\n  \"description\": \"GetBlueprintRunResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlueprintRun\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlueprintRun\"\n        },\n        {\n          \"description\": \"Returns a <code>BlueprintRun</code> object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-blueprint-run-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetBlueprintRunResponse
---
