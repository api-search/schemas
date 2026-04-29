---
description: ListBlueprintsResponse schema from Amazon Glue API
layout: schema
name: ListBlueprintsResponse
properties_list:
- description: ''
  name: Blueprints
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-blueprints-response-schema.json
slug: glue-list-blueprints-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-blueprints-response-schema.json\",\n  \"title\": \"ListBlueprintsResponse\",\n  \"description\": \"ListBlueprintsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Blueprints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlueprintNames\"\n        },\n        {\n          \"description\": \"List of names of blueprints in the account.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if not all blueprint names have been returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-blueprints-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListBlueprintsResponse
---
