---
description: The result returned by the Apidog API after an import operation (OpenAPI, Swagger, or Postman Collection).
layout: schema
name: Apidog Import Result
properties_list:
- description: Whether the import operation completed successfully.
  name: success
  type: boolean
- description: Details about the imported resources.
  name: data
  type: object
provider_name: Apidog
provider_slug: apidog
schema_file: json-schema/apidog-import-result-schema.json
slug: apidog-import-result
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apidog/refs/heads/main/json-schema/apidog-import-result-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Apidog Import Result\",\n  \"description\": \"The result returned by the Apidog API after an import operation (OpenAPI, Swagger, or Postman Collection).\",\n  \"type\": \"object\",\n  \"required\": [\n    \"success\"\n  ],\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the import operation completed successfully.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Details about the imported resources.\",\n      \"properties\": {\n        \"endpointCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of endpoints imported.\",\n          \"minimum\": 0\n        },\n        \"schemaCount\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Number of schemas imported.\",\n          \"minimum\": 0\n        },\n        \"environmentCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of environments imported.\",\n          \"minimum\": 0\n        }\n      },\n      \"additionalProperties\": false\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apidog/refs/heads/main/json-schema/apidog-import-result-schema.json
tags:
- API Design
- API Lifecycle
- API Testing
- Collaboration
- Design-First
- Documentation
- Mocking
- Platform
title: Apidog Import Result
---
