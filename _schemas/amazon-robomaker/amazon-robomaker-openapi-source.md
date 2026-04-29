---
description: Information about a source.
layout: schema
name: Source
properties_list:
- description: ''
  name: s3Bucket
  type: object
- description: ''
  name: s3Key
  type: object
- description: ''
  name: etag
  type: object
- description: ''
  name: architecture
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-source-schema.json
slug: amazon-robomaker-openapi-source
source_filename: amazon-robomaker-openapi-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-source-schema.json\",\n  \"title\": \"Source\",\n  \"description\": \"Information about a source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Bucket\"\n        },\n        {\n          \"description\": \"The s3 bucket name.\"\n        }\n      ]\n    },\n    \"s3Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Key\"\n        },\n        {\n          \"description\": \"The s3 object key.\"\n        }\n      ]\n    },\n    \"etag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Etag\"\n        },\n        {\n          \"description\": \"A hash of the object specified by <code>s3Bucket</code> and <code>s3Key</code>.\"\
  \n        }\n      ]\n    },\n    \"architecture\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Architecture\"\n        },\n        {\n          \"description\": \"The taget processor architecture for the application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-source-schema.json
tags:
- AWS
- Robotics
- Simulation
title: Source
---
