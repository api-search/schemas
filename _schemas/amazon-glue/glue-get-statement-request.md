---
description: GetStatementRequest schema from Amazon Glue API
layout: schema
name: GetStatementRequest
properties_list:
- description: ''
  name: SessionId
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: RequestOrigin
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-statement-request-schema.json
slug: glue-get-statement-request
source_filename: glue-get-statement-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-statement-request-schema.json\",\n  \"title\": \"GetStatementRequest\",\n  \"description\": \"GetStatementRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The Session ID of the statement.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerValue\"\n        },\n        {\n          \"description\": \"The Id of the statement.\"\n        }\n      ]\n    },\n    \"RequestOrigin\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrchestrationNameString\"\n        },\n        {\n          \"description\":\
  \ \"The origin of the request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SessionId\",\n    \"Id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-statement-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetStatementRequest
---
