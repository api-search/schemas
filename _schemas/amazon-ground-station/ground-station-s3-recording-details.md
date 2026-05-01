---
description: Details about an S3 recording <code>Config</code> used in a contact.
layout: schema
name: S3RecordingDetails
properties_list:
- description: ''
  name: bucketArn
  type: object
- description: ''
  name: keyTemplate
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-s3-recording-details-schema.json
slug: ground-station-s3-recording-details
source_filename: ground-station-s3-recording-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-s3-recording-details-schema.json\",\n  \"title\": \"S3RecordingDetails\",\n  \"description\": \"Details about an S3 recording <code>Config</code> used in a contact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketArn\"\n        },\n        {\n          \"description\": \"ARN of the bucket used.\"\n        }\n      ]\n    },\n    \"keyTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Key template used for the S3 Recording Configuration\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-s3-recording-details-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: S3RecordingDetails
---
