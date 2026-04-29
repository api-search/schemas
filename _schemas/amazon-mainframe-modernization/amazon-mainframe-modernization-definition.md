---
description: The application definition for a particular application.
layout: schema
name: Definition
properties_list:
- description: ''
  name: content
  type: object
- description: ''
  name: s3Location
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-definition-schema.json
slug: amazon-mainframe-modernization-definition
source_filename: amazon-mainframe-modernization-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-definition-schema.json\",\n  \"title\": \"Definition\",\n  \"description\": \"The application definition for a particular application. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFree65000\"\n        },\n        {\n          \"description\": \"The content of the application definition. This is a JSON object that contains the resource configuration/definitions that identify an application.\"\n        }\n      ]\n    },\n    \"s3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String2000\"\n        },\n        {\n          \"description\": \"The S3 bucket that contains the application definition.\"\n        }\n   \
  \   ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-definition-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: Definition
---
