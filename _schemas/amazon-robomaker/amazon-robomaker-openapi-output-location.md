---
description: The output location.
layout: schema
name: OutputLocation
properties_list:
- description: ''
  name: s3Bucket
  type: object
- description: ''
  name: s3Prefix
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-output-location-schema.json
slug: amazon-robomaker-openapi-output-location
source_filename: amazon-robomaker-openapi-output-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-output-location-schema.json\",\n  \"title\": \"OutputLocation\",\n  \"description\": \"The output location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Bucket\"\n        },\n        {\n          \"description\": \"The S3 bucket for output.\"\n        }\n      ]\n    },\n    \"s3Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Key\"\n        },\n        {\n          \"description\": \"The S3 folder in the <code>s3Bucket</code> where output files will be placed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-output-location-schema.json
tags:
- AWS
- Robotics
- Simulation
title: OutputLocation
---
