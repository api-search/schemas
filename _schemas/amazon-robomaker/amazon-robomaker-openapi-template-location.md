---
description: Information about a template location.
layout: schema
name: TemplateLocation
properties_list:
- description: ''
  name: s3Bucket
  type: object
- description: ''
  name: s3Key
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-template-location-schema.json
slug: amazon-robomaker-openapi-template-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-template-location-schema.json\",\n  \"title\": \"TemplateLocation\",\n  \"description\": \"Information about a template location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Bucket\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket name.\"\n        }\n      ]\n    },\n    \"s3Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Key\"\n        },\n        {\n          \"description\": \"The list of S3 keys identifying the data source files.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"s3Bucket\",\n    \"s3Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-template-location-schema.json
tags:
- AWS
- Robotics
- Simulation
title: TemplateLocation
---
