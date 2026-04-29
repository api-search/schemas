---
description: Object stored in S3 containing ephemeris data.
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
  name: version
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-s3-object-schema.json
slug: ground-station-s3-object
source_filename: ground-station-s3-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-s3-object-schema.json\",\n  \"title\": \"S3Object\",\n  \"description\": \"Object stored in S3 containing ephemeris data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\n        },\n        {\n          \"description\": \"An Amazon S3 Bucket name.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ObjectKey\"\n        },\n        {\n          \"description\": \"An Amazon S3 key for the ephemeris.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3VersionId\"\n        },\n        {\n          \"description\": \"For versioned S3\
  \ objects, the version to use for the ephemeris.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-s3-object-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: S3Object
---
