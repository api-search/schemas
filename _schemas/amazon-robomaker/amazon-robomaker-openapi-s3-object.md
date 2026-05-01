---
description: Information about an S3 object.
layout: schema
name: S3Object
properties_list:
- description: ''
  name: bucket
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: etag
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-s3-object-schema.json
slug: amazon-robomaker-openapi-s3-object
source_filename: amazon-robomaker-openapi-s3-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-s3-object-schema.json\",\n  \"title\": \"S3Object\",\n  \"description\": \"Information about an S3 object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Bucket\"\n        },\n        {\n          \"description\": \"The bucket containing the object.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Key\"\n        },\n        {\n          \"description\": \"The key of the object.\"\n        }\n      ]\n    },\n    \"etag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Etag\"\n        },\n        {\n          \"description\": \"The etag of the object.\"\n        }\n      ]\n  \
  \  }\n  },\n  \"required\": [\n    \"bucket\",\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-s3-object-schema.json
tags:
- Robotics
- Simulation
title: S3Object
---
