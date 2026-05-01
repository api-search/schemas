---
description: Configuration parameters for where in an S3 bucket to place the harvested content
layout: schema
name: S3Destination
properties_list:
- description: ''
  name: BucketName
  type: object
- description: ''
  name: ManifestKey
  type: object
- description: ''
  name: RoleArn
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-s3-destination-schema.json
slug: mediapackage-api-s3-destination
source_filename: mediapackage-api-s3-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-s3-destination-schema.json\",\n  \"title\": \"S3Destination\",\n  \"description\": \"Configuration parameters for where in an S3 bucket to place the harvested content\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bucketName\"\n          },\n          \"description\": \"The name of an S3 bucket within which harvested content will be exported\\n\"\n        }\n      ]\n    },\n    \"ManifestKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestKey\"\n          },\n          \"description\"\
  : \"The key in the specified S3 bucket where the harvested top-level manifest will be placed.\\n\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"roleArn\"\n          },\n          \"description\": \"The IAM role used to write to the specified S3 bucket\\n\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ManifestKey\",\n    \"BucketName\",\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-s3-destination-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: S3Destination
---
