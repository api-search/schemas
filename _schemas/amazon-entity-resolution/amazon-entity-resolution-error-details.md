---
description: An object containing an error message, if there was an error.
layout: schema
name: ErrorDetails
properties_list:
- description: ''
  name: errorMessage
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-error-details-schema.json
slug: amazon-entity-resolution-error-details
source_filename: amazon-entity-resolution-error-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-error-details-schema.json\",\n  \"title\": \"ErrorDetails\",\n  \"description\": \"An object containing an error message, if there was an error.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorMessage\"\n        },\n        {\n          \"description\": \"The error message from the job, if there is one.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-error-details-schema.json
tags:
- Amazon Web Services
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: ErrorDetails
---
