---
description: StopApplicationRequest schema from AWS Mainframe Modernization API
layout: schema
name: StopApplicationRequest
properties_list:
- description: ''
  name: forceStop
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-stop-application-request-schema.json
slug: amazon-mainframe-modernization-stop-application-request
source_filename: amazon-mainframe-modernization-stop-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-stop-application-request-schema.json\",\n  \"title\": \"StopApplicationRequest\",\n  \"description\": \"StopApplicationRequest schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"forceStop\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Stopping an application process can take a long time. Setting this parameter to true lets you force stop the application so you don't need to wait until the process finishes to apply another action on the application. The default value is false.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-stop-application-request-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: StopApplicationRequest
---
