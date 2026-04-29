---
description: A request to create a partner input
layout: schema
name: CreatePartnerInputRequest
properties_list:
- description: ''
  name: RequestId
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-create-partner-input-request-schema.json
slug: medialive-api-create-partner-input-request
source_filename: medialive-api-create-partner-input-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-partner-input-request-schema.json\",\n  \"title\": \"CreatePartnerInputRequest\",\n  \"description\": \"A request to create a partner input\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"requestId\"\n          },\n          \"description\": \"Unique identifier of the request to ensure the request is handled\\nexactly once in case of retries.\\n\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A collection of\
  \ key-value pairs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-partner-input-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreatePartnerInputRequest
---
