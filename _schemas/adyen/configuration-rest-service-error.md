---
description: RestServiceError schema from Adyen API
layout: schema
name: RestServiceError
properties_list:
- description: A human-readable explanation specific to this occurrence of the problem.
  name: detail
  type: string
- description: A code that identifies the problem type.
  name: errorCode
  type: string
- description: A unique URI that identifies the specific occurrence of the problem.
  name: instance
  type: string
- description: Detailed explanation of each validation error, when applicable.
  name: invalidFields
  type: array
- description: A unique reference for the request, essentially the same as `pspReference`.
  name: requestId
  type: string
- description: JSON response payload.
  name: response
  type: object
- description: The HTTP status code.
  name: status
  type: integer
- description: A short, human-readable summary of the problem type.
  name: title
  type: string
- description: A URI that identifies the problem type, pointing to human-readable documentation on this problem type.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-rest-service-error-schema.json
slug: configuration-rest-service-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-rest-service-error-schema.json\",\n  \"title\": \"RestServiceError\",\n  \"description\": \"RestServiceError schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detail\": {\n      \"description\": \"A human-readable explanation specific to this occurrence of the problem.\",\n      \"type\": \"string\"\n    },\n    \"errorCode\": {\n      \"description\": \"A code that identifies the problem type.\",\n      \"type\": \"string\"\n    },\n    \"instance\": {\n      \"description\": \"A unique URI that identifies the specific occurrence of the problem.\",\n      \"type\": \"string\"\n    },\n    \"invalidFields\": {\n      \"description\": \"Detailed explanation of each validation error, when applicable.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InvalidField\"\
  \n      },\n      \"type\": \"array\"\n    },\n    \"requestId\": {\n      \"description\": \"A unique reference for the request, essentially the same as `pspReference`.\",\n      \"type\": \"string\"\n    },\n    \"response\": {\n      \"description\": \"JSON response payload.\",\n      \"$ref\": \"#/components/schemas/JSONObject\"\n    },\n    \"status\": {\n      \"description\": \"The HTTP status code.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"title\": {\n      \"description\": \"A short, human-readable summary of the problem type.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"A URI that identifies the problem type, pointing to human-readable documentation on this problem type.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"errorCode\",\n    \"title\",\n    \"detail\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-rest-service-error-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RestServiceError
---
