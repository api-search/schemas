---
description: Information about an S3 recording <code>Config</code>.
layout: schema
name: S3RecordingConfig
properties_list:
- description: ''
  name: bucketArn
  type: object
- description: ''
  name: prefix
  type: object
- description: ''
  name: roleArn
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-s3-recording-config-schema.json
slug: ground-station-s3-recording-config
source_filename: ground-station-s3-recording-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-s3-recording-config-schema.json\",\n  \"title\": \"S3RecordingConfig\",\n  \"description\": \"Information about an S3 recording <code>Config</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketArn\"\n        },\n        {\n          \"description\": \"ARN of the bucket to record to.\"\n        }\n      ]\n    },\n    \"prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3KeyPrefix\"\n        },\n        {\n          \"description\": \"S3 Key prefix to prefice data files.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"\
  description\": \"ARN of the role Ground Station assumes to write data to the bucket.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bucketArn\",\n    \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-s3-recording-config-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: S3RecordingConfig
---
