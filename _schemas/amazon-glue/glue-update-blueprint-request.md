---
description: UpdateBlueprintRequest schema from Amazon Glue API
layout: schema
name: UpdateBlueprintRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: BlueprintLocation
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-blueprint-request-schema.json
slug: glue-update-blueprint-request
source_filename: glue-update-blueprint-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-blueprint-request-schema.json\",\n  \"title\": \"UpdateBlueprintRequest\",\n  \"description\": \"UpdateBlueprintRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrchestrationNameString\"\n        },\n        {\n          \"description\": \"The name of the blueprint.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Generic512CharString\"\n        },\n        {\n          \"description\": \"A description of the blueprint.\"\n        }\n      ]\n    },\n    \"BlueprintLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrchestrationS3Location\"\n        },\n\
  \        {\n          \"description\": \"Specifies a path in Amazon S3 where the blueprint is published.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"BlueprintLocation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-blueprint-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateBlueprintRequest
---
