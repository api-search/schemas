---
description: ''
layout: schema
name: CreateRunGroupResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-create-run-group-response-schema.json
slug: healthomics-create-run-group-response
source_filename: healthomics-create-run-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-run-group-response-schema.json\",\n  \"title\": \"CreateRunGroupResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupArn\"\n        },\n        {\n          \"description\": \"The group's ARN.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupId\"\n        },\n        {\n          \"description\": \"The group's ID.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags for the run group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-run-group-response-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: CreateRunGroupResponse
---
