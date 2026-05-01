---
description: Placeholder documentation for BatchDeleteResponse
layout: schema
name: BatchDeleteResponse
properties_list:
- description: ''
  name: Failed
  type: object
- description: ''
  name: Successful
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-batch-delete-response-schema.json
slug: medialive-api-batch-delete-response
source_filename: medialive-api-batch-delete-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-delete-response-schema.json\",\n  \"title\": \"BatchDeleteResponse\",\n  \"description\": \"Placeholder documentation for BatchDeleteResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Failed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfBatchFailedResultModel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"failed\"\n          },\n          \"description\": \"List of failed operations\"\n        }\n      ]\n    },\n    \"Successful\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfBatchSuccessfulResultModel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"successful\"\n          },\n          \"description\": \"List of successful operations\"\n\
  \        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-delete-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: BatchDeleteResponse
---
