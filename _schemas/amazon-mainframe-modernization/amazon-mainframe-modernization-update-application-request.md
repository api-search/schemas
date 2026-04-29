---
description: UpdateApplicationRequest schema from AWS Mainframe Modernization API
layout: schema
name: UpdateApplicationRequest
properties_list:
- description: ''
  name: currentApplicationVersion
  type: object
- description: ''
  name: definition
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-update-application-request-schema.json
slug: amazon-mainframe-modernization-update-application-request
source_filename: amazon-mainframe-modernization-update-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-update-application-request-schema.json\",\n  \"title\": \"UpdateApplicationRequest\",\n  \"description\": \"UpdateApplicationRequest schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentApplicationVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The current version of the application to update.\"\n        }\n      ]\n    },\n    \"definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Definition\"\n        },\n        {\n          \"description\": \"The application definition for this application. You can specify either inline JSON or an S3 bucket location.\"\n       \
  \ }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityDescription\"\n        },\n        {\n          \"description\": \"The description of the application to update.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"currentApplicationVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-update-application-request-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: UpdateApplicationRequest
---
