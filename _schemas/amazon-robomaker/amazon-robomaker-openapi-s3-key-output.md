---
description: Information about S3 keys.
layout: schema
name: S3KeyOutput
properties_list:
- description: ''
  name: s3Key
  type: object
- description: ''
  name: etag
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-s3-key-output-schema.json
slug: amazon-robomaker-openapi-s3-key-output
source_filename: amazon-robomaker-openapi-s3-key-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-s3-key-output-schema.json\",\n  \"title\": \"S3KeyOutput\",\n  \"description\": \"Information about S3 keys.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3KeyOrPrefix\"\n        },\n        {\n          \"description\": \"The S3 key.\"\n        }\n      ]\n    },\n    \"etag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Etag\"\n        },\n        {\n          \"description\": \"The etag for the object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-s3-key-output-schema.json
tags:
- AWS
- Robotics
- Simulation
title: S3KeyOutput
---
