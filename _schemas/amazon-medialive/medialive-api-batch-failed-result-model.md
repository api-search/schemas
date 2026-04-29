---
description: Details from a failed operation
layout: schema
name: BatchFailedResultModel
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Code
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-batch-failed-result-model-schema.json
slug: medialive-api-batch-failed-result-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-failed-result-model-schema.json\",\n  \"title\": \"BatchFailedResultModel\",\n  \"description\": \"Details from a failed operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"ARN of the resource\"\n        }\n      ]\n    },\n    \"Code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"code\"\n          },\n          \"description\": \"Error code for the failed operation\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"ID of the resource\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"message\"\n          },\n          \"description\": \"Error message for the failed operation\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-failed-result-model-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BatchFailedResultModel
---
