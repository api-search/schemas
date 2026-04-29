---
description: CreateApplicationResponse schema from AWS Mainframe Modernization API
layout: schema
name: CreateApplicationResponse
properties_list:
- description: ''
  name: applicationArn
  type: object
- description: ''
  name: applicationId
  type: object
- description: ''
  name: applicationVersion
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-create-application-response-schema.json
slug: amazon-mainframe-modernization-create-application-response
source_filename: amazon-mainframe-modernization-create-application-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-application-response-schema.json\",\n  \"title\": \"CreateApplicationResponse\",\n  \"description\": \"CreateApplicationResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the application.\"\n        }\n      ]\n    },\n    \"applicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique application identifier.\"\n        }\n      ]\n    },\n    \"applicationVersion\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version number of the application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationArn\",\n    \"applicationId\",\n    \"applicationVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-application-response-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: CreateApplicationResponse
---
