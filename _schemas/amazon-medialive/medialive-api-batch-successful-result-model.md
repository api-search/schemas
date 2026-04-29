---
description: Details from a successful operation
layout: schema
name: BatchSuccessfulResultModel
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: State
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-batch-successful-result-model-schema.json
slug: medialive-api-batch-successful-result-model
source_filename: medialive-api-batch-successful-result-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-successful-result-model-schema.json\",\n  \"title\": \"BatchSuccessfulResultModel\",\n  \"description\": \"Details from a successful operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"ARN of the resource\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"ID of the resource\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          },\n          \"description\": \"Current state of the resource\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-successful-result-model-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BatchSuccessfulResultModel
---
