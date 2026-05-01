---
description: RunStatementRequest schema from Amazon Glue API
layout: schema
name: RunStatementRequest
properties_list:
- description: ''
  name: SessionId
  type: object
- description: ''
  name: Code
  type: object
- description: ''
  name: RequestOrigin
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-run-statement-request-schema.json
slug: glue-run-statement-request
source_filename: glue-run-statement-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-run-statement-request-schema.json\",\n  \"title\": \"RunStatementRequest\",\n  \"description\": \"RunStatementRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The Session Id of the statement to be run.\"\n        }\n      ]\n    },\n    \"Code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrchestrationStatementCodeString\"\n        },\n        {\n          \"description\": \"The statement code to be run.\"\n        }\n      ]\n    },\n    \"RequestOrigin\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrchestrationNameString\"\n        },\n\
  \        {\n          \"description\": \"The origin of the request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SessionId\",\n    \"Code\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-run-statement-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: RunStatementRequest
---
