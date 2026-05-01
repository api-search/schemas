---
description: DeleteMatchingWorkflowOutput schema from AWS EntityResolution
layout: schema
name: DeleteMatchingWorkflowOutput
properties_list:
- description: ''
  name: message
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-delete-matching-workflow-output-schema.json
slug: amazon-entity-resolution-delete-matching-workflow-output
source_filename: amazon-entity-resolution-delete-matching-workflow-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-delete-matching-workflow-output-schema.json\",\n  \"title\": \"DeleteMatchingWorkflowOutput\",\n  \"description\": \"DeleteMatchingWorkflowOutput schema from AWS EntityResolution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A successful operation message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-delete-matching-workflow-output-schema.json
tags:
- Amazon Web Services
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: DeleteMatchingWorkflowOutput
---
