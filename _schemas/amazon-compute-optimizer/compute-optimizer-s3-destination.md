---
description: Describes the destination Amazon Simple Storage Service (Amazon S3) bucket name and object keys of a recommendations export file, and its associated metadata file.
layout: schema
name: S3Destination
properties_list:
- description: ''
  name: bucket
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: metadataKey
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-s3-destination-schema.json
slug: compute-optimizer-s3-destination
source_filename: compute-optimizer-s3-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-s3-destination-schema.json\",\n  \"title\": \"S3Destination\",\n  \"description\": \"Describes the destination Amazon Simple Storage Service (Amazon S3) bucket name and object keys of a recommendations export file, and its associated metadata file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationBucket\"\n        },\n        {\n          \"description\": \"The name of the Amazon S3 bucket used as the destination of an export file.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationKey\"\n        },\n        {\n          \"description\": \"<p>The Amazon S3 bucket key of an export file.</p> <p>The\
  \ key uniquely identifies the object, or export file, in the S3 bucket.</p>\"\n        }\n      ]\n    },\n    \"metadataKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetadataKey\"\n        },\n        {\n          \"description\": \"<p>The Amazon S3 bucket key of a metadata file.</p> <p>The key uniquely identifies the object, or metadata file, in the S3 bucket.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-s3-destination-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: S3Destination
---
