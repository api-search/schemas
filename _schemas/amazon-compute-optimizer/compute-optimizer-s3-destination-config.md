---
description: <p>Describes the destination Amazon Simple Storage Service (Amazon S3) bucket name and key prefix for a recommendations export job.</p> <p>You must create the destination Amazon S3 bucket for your recommendations export before you create the export job. Compute Optimizer does not create the S3 bucket for you. After you create the S3 bucket, ensure that it has the required permission policy to allow Compute Optimizer to write the export file to it. If you plan to specify an object prefix when you create the export job, you must include the object prefix in the policy that you add to the S3 bucket. For more information, see <a href="https://docs.aws.amazon.com/compute-optimizer/latest/ug/create-s3-bucket-policy-for-compute-optimizer.html">Amazon S3 Bucket Policy for Compute Optimizer</a> in the <i>Compute Optimizer User Guide</i>.</p>
layout: schema
name: S3DestinationConfig
properties_list:
- description: ''
  name: bucket
  type: object
- description: ''
  name: keyPrefix
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-s3-destination-config-schema.json
slug: compute-optimizer-s3-destination-config
source_filename: compute-optimizer-s3-destination-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-s3-destination-config-schema.json\",\n  \"title\": \"S3DestinationConfig\",\n  \"description\": \"<p>Describes the destination Amazon Simple Storage Service (Amazon S3) bucket name and key prefix for a recommendations export job.</p> <p>You must create the destination Amazon S3 bucket for your recommendations export before you create the export job. Compute Optimizer does not create the S3 bucket for you. After you create the S3 bucket, ensure that it has the required permission policy to allow Compute Optimizer to write the export file to it. If you plan to specify an object prefix when you create the export job, you must include the object prefix in the policy that you add to the S3 bucket. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/create-s3-bucket-policy-for-compute-optimizer.html\\\
  \">Amazon S3 Bucket Policy for Compute Optimizer</a> in the <i>Compute Optimizer User Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationBucket\"\n        },\n        {\n          \"description\": \"The name of the Amazon S3 bucket to use as the destination for an export job.\"\n        }\n      ]\n    },\n    \"keyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationKeyPrefix\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket prefix for an export job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-s3-destination-config-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: S3DestinationConfig
---
