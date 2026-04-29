---
description: Information about a source configuration.
layout: schema
name: SourceConfig
properties_list:
- description: ''
  name: s3Bucket
  type: object
- description: ''
  name: s3Key
  type: object
- description: ''
  name: architecture
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-source-config-schema.json
slug: amazon-robomaker-openapi-source-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-source-config-schema.json\",\n  \"title\": \"SourceConfig\",\n  \"description\": \"Information about a source configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Bucket\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket name.\"\n        }\n      ]\n    },\n    \"s3Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Key\"\n        },\n        {\n          \"description\": \"The s3 object key.\"\n        }\n      ]\n    },\n    \"architecture\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Architecture\"\n        },\n        {\n          \"description\": \"The target processor architecture\
  \ for the application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-source-config-schema.json
tags:
- AWS
- Robotics
- Simulation
title: SourceConfig
---
