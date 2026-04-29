---
description: GetCustomEntityTypeResponse schema from Amazon Glue API
layout: schema
name: GetCustomEntityTypeResponse
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RegexString
  type: object
- description: ''
  name: ContextWords
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-custom-entity-type-response-schema.json
slug: glue-get-custom-entity-type-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-custom-entity-type-response-schema.json\",\n  \"title\": \"GetCustomEntityTypeResponse\",\n  \"description\": \"GetCustomEntityTypeResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the custom pattern that you retrieved.\"\n        }\n      ]\n    },\n    \"RegexString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"A regular expression string that is used for detecting sensitive data in a custom pattern.\"\n        }\n      ]\n    },\n    \"ContextWords\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/ContextWords\"\n        },\n        {\n          \"description\": \"A list of context words if specified when you created the custom pattern. If none of these context words are found within the vicinity of the regular expression the data will not be detected as sensitive data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-custom-entity-type-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetCustomEntityTypeResponse
---
