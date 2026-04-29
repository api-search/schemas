---
description: GetApplicationVersionResponse schema from AWS Mainframe Modernization API
layout: schema
name: GetApplicationVersionResponse
properties_list:
- description: ''
  name: applicationVersion
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: definitionContent
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusReason
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-get-application-version-response-schema.json
slug: amazon-mainframe-modernization-get-application-version-response
source_filename: amazon-mainframe-modernization-get-application-version-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-get-application-version-response-schema.json\",\n  \"title\": \"GetApplicationVersionResponse\",\n  \"description\": \"GetApplicationVersionResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The specific version of the application.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when the application version was created.\"\n        }\n      ]\n    },\n    \"definitionContent\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFree65000\"\n        },\n        {\n          \"description\": \"The content of the application definition. This is a JSON object that contains the resource configuration and definitions that identify an application.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityDescription\"\n        },\n        {\n          \"description\": \"The application description.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the application version.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionLifecycle\"\n        },\n        {\n          \"description\": \"The status of the application version.\"\n\
  \        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The reason for the reported status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationVersion\",\n    \"creationTime\",\n    \"definitionContent\",\n    \"name\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-get-application-version-response-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: GetApplicationVersionResponse
---
