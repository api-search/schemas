---
description: GetSensitiveDataOccurrencesResponse schema from Amazon Macie API
layout: schema
name: GetSensitiveDataOccurrencesResponse
properties_list:
- description: ''
  name: error
  type: object
- description: ''
  name: sensitiveDataOccurrences
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-sensitive-data-occurrences-response-schema.json
slug: amazon-macie-get-sensitive-data-occurrences-response
source_filename: amazon-macie-get-sensitive-data-occurrences-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-sensitive-data-occurrences-response-schema.json\",\n  \"title\": \"GetSensitiveDataOccurrencesResponse\",\n  \"description\": \"GetSensitiveDataOccurrencesResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"If an error occurred when Amazon Macie attempted to retrieve occurrences of sensitive data reported by the finding, a description of the error that occurred. This value is null if the status (status) of the request is PROCESSING or SUCCESS.\"\n        }\n      ]\n    },\n    \"sensitiveDataOccurrences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveDataOccurrences\"\
  \n        },\n        {\n          \"description\": \"A map that specifies 1-100 types of sensitive data reported by the finding and, for each type, 1-10 occurrences of sensitive data.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevealRequestStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the request to retrieve occurrences of sensitive data reported by the finding. Possible values are:</p> <ul><li><p>ERROR - An error occurred when Amazon Macie attempted to locate, retrieve, or encrypt the sensitive data. The error value indicates the nature of the error that occurred.</p></li> <li><p>PROCESSING - Macie is processing the request.</p></li> <li><p>SUCCESS - Macie successfully located, retrieved, and encrypted the sensitive data.</p></li></ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-sensitive-data-occurrences-response-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetSensitiveDataOccurrencesResponse
---
