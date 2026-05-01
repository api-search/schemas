---
description: GetBlueprintRunsResponse schema from Amazon Glue API
layout: schema
name: GetBlueprintRunsResponse
properties_list:
- description: ''
  name: BlueprintRuns
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-blueprint-runs-response-schema.json
slug: glue-get-blueprint-runs-response
source_filename: glue-get-blueprint-runs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-blueprint-runs-response-schema.json\",\n  \"title\": \"GetBlueprintRunsResponse\",\n  \"description\": \"GetBlueprintRunsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlueprintRuns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlueprintRuns\"\n        },\n        {\n          \"description\": \"Returns a list of <code>BlueprintRun</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if not all blueprint runs have been returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-blueprint-runs-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetBlueprintRunsResponse
---
