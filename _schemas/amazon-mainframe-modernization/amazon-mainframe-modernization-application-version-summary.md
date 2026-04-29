---
description: Defines an application version summary.
layout: schema
name: ApplicationVersionSummary
properties_list:
- description: ''
  name: applicationVersion
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusReason
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-application-version-summary-schema.json
slug: amazon-mainframe-modernization-application-version-summary
source_filename: amazon-mainframe-modernization-application-version-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-application-version-summary-schema.json\",\n  \"title\": \"ApplicationVersionSummary\",\n  \"description\": \"Defines an application version summary.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The application version.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when the application version was created.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionLifecycle\"\
  \n        },\n        {\n          \"description\": \"The status of the application.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The reason for the reported status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationVersion\",\n    \"creationTime\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-application-version-summary-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: ApplicationVersionSummary
---
