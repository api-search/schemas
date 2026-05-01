---
description: ''
layout: schema
name: UntagResourceRequest
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-untag-resource-request-schema.json
slug: healthlake-untag-resource-request
source_filename: healthlake-untag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-untag-resource-request-schema.json\",\n  \"title\": \"UntagResourceRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceARN\",\n    \"TagKeys\"\n  ],\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name(ARN) of the data store for which tags are being removed.\"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeyList\"\n        },\n        {\n          \"description\": \" The keys for the tags to be removed from the HealthLake data store. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-untag-resource-request-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: UntagResourceRequest
---
