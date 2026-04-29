---
description: A complex type that describes an S3 location where recorded videos will be stored.
layout: schema
name: S3DestinationConfiguration
properties_list:
- description: ''
  name: bucketName
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-s3-destination-configuration-schema.json
slug: ivs-s3-destination-configuration
source_filename: ivs-s3-destination-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-s3-destination-configuration-schema.json\",\n  \"title\": \"S3DestinationConfiguration\",\n  \"description\": \"A complex type that describes an S3 location where recorded videos will be stored.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3DestinationBucketName\"\n        },\n        {\n          \"description\": \"Location (S3 bucket name) where recorded videos will be stored.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bucketName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-s3-destination-configuration-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: S3DestinationConfiguration
---
