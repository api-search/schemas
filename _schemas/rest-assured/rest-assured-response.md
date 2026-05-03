---
description: Schema for a REST Assured response validation specification, representing the then() clause of a REST Assured test.
layout: schema
name: REST Assured Response Specification
properties_list:
- description: Expected HTTP status code of the response.
  name: statusCode
  type: integer
- description: Expected Content-Type of the response.
  name: contentType
  type: string
- description: Expected HTTP response headers and their values.
  name: headers
  type: object
- description: Expected body assertions using JSONPath expressions.
  name: body
  type: object
- description: Response time constraint.
  name: responseTime
  type: object
- description: Expected cookies in the response.
  name: cookies
  type: object
provider_name: REST Assured
provider_slug: rest-assured
schema_file: json-schema/rest-assured-response-schema.json
slug: rest-assured-response
source_filename: rest-assured-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://rest-assured.io/schemas/response\",\n  \"title\": \"REST Assured Response Specification\",\n  \"description\": \"Schema for a REST Assured response validation specification, representing the then() clause of a REST Assured test.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"minimum\": 100,\n      \"maximum\": 599,\n      \"description\": \"Expected HTTP status code of the response.\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"Expected Content-Type of the response.\",\n      \"examples\": [\"application/json\", \"application/xml\"]\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Expected HTTP response headers and their values.\"\n    },\n    \"body\": {\n      \"type\": \"\
  object\",\n      \"description\": \"Expected body assertions using JSONPath expressions.\",\n      \"additionalProperties\": true\n    },\n    \"responseTime\": {\n      \"type\": \"object\",\n      \"description\": \"Response time constraint.\",\n      \"properties\": {\n        \"lessThan\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum acceptable response time in milliseconds.\"\n        },\n        \"greaterThan\": {\n          \"type\": \"integer\",\n          \"description\": \"Minimum acceptable response time in milliseconds.\"\n        }\n      }\n    },\n    \"cookies\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Expected cookies in the response.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rest-assured/refs/heads/main/json-schema/rest-assured-response-schema.json
tags:
- Functional Testing
- Testing
- Java
- API Testing
- Automation
title: REST Assured Response Specification
---
