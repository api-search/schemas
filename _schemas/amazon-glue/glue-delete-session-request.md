---
description: DeleteSessionRequest schema from Amazon Glue API
layout: schema
name: DeleteSessionRequest
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: RequestOrigin
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-session-request-schema.json
slug: glue-delete-session-request
source_filename: glue-delete-session-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-session-request-schema.json\",\n  \"title\": \"DeleteSessionRequest\",\n  \"description\": \"DeleteSessionRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The ID of the session to be deleted.\"\n        }\n      ]\n    },\n    \"RequestOrigin\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrchestrationNameString\"\n        },\n        {\n          \"description\": \"The name of the origin of the delete session request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-session-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteSessionRequest
---
