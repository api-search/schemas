---
description: DeleteBlueprintResponse schema from Amazon Glue API
layout: schema
name: DeleteBlueprintResponse
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-blueprint-response-schema.json
slug: glue-delete-blueprint-response
source_filename: glue-delete-blueprint-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-blueprint-response-schema.json\",\n  \"title\": \"DeleteBlueprintResponse\",\n  \"description\": \"DeleteBlueprintResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Returns the name of the blueprint that was deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-blueprint-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteBlueprintResponse
---
