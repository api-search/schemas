---
description: An Amazon S3 bucket and optional folder (object key prefix) where SimSpace Weaver creates a file.
layout: schema
name: S3Destination
properties_list:
- description: ''
  name: BucketName
  type: object
- description: ''
  name: ObjectKeyPrefix
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-s3-destination-schema.json
slug: amazon-simspace-weaver-s3-destination
source_filename: amazon-simspace-weaver-s3-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-s3-destination-schema.json\",\n  \"title\": \"S3Destination\",\n  \"description\": \"An Amazon S3 bucket and optional folder (object key prefix) where SimSpace Weaver creates a file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketName\"\n        },\n        {\n          \"description\": \"The name of an Amazon S3 bucket. For more information about buckets, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-buckets-s3.html\\\">Creating, configuring, and working with Amazon S3 buckets</a> in the <i>Amazon Simple Storage Service User Guide</i>.\"\n        }\n      ]\n    },\n    \"ObjectKeyPrefix\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/ObjectKeyPrefix\"\n        },\n        {\n          \"description\": \"A string prefix for an Amazon S3 object key. It's usually a folder name. For more information about folders in Amazon S3, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/using-folders.html\\\">Organizing objects in the Amazon S3 console using folders</a> in the <i>Amazon Simple Storage Service User Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-s3-destination-schema.json
tags:
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: S3Destination
---
