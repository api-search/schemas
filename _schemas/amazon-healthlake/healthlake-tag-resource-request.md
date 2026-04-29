---
description: ''
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-tag-resource-request-schema.json
slug: healthlake-tag-resource-request
source_filename: healthlake-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceARN\",\n    \"Tags\"\n  ],\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name(ARN)that gives AWS HealthLake access to the data store which tags are being added to. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \" The user specified key and value pair tags being added to a data store. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-tag-resource-request-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: TagResourceRequest
---
