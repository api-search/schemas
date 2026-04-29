---
description: GetUserDefinedFunctionsResponse schema from Amazon Glue API
layout: schema
name: GetUserDefinedFunctionsResponse
properties_list:
- description: ''
  name: UserDefinedFunctions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-user-defined-functions-response-schema.json
slug: glue-get-user-defined-functions-response
source_filename: glue-get-user-defined-functions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-user-defined-functions-response-schema.json\",\n  \"title\": \"GetUserDefinedFunctionsResponse\",\n  \"description\": \"GetUserDefinedFunctionsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserDefinedFunctions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserDefinedFunctionList\"\n        },\n        {\n          \"description\": \"A list of requested function definitions.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if the list of functions returned does not include the last requested function.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-user-defined-functions-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetUserDefinedFunctionsResponse
---
