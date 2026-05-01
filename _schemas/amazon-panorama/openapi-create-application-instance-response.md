---
description: CreateApplicationInstanceResponse schema from Amazon Panorama
layout: schema
name: CreateApplicationInstanceResponse
properties_list:
- description: ''
  name: ApplicationInstanceId
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-create-application-instance-response-schema.json
slug: openapi-create-application-instance-response
source_filename: openapi-create-application-instance-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-application-instance-response-schema.json\",\n  \"title\": \"CreateApplicationInstanceResponse\",\n  \"description\": \"CreateApplicationInstanceResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationInstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceId\"\n        },\n        {\n          \"description\": \"The application instance's ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationInstanceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-application-instance-response-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: CreateApplicationInstanceResponse
---
