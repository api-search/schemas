---
description: Contains an array of Amazon Web Services resource objects. Each object represents an Amazon S3 bucket, an Lambda function, or an Amazon Machine Image (AMI) based on Amazon EC2 that is associated with a particular job.
layout: schema
name: JobResource
properties_list:
- description: ''
  name: S3Resources
  type: object
- description: ''
  name: LambdaResources
  type: object
- description: ''
  name: Ec2AmiResources
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-job-resource-schema.json
slug: amazon-snow-family-job-resource
source_filename: amazon-snow-family-job-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-job-resource-schema.json\",\n  \"title\": \"JobResource\",\n  \"description\": \"Contains an array of Amazon Web Services resource objects. Each object represents an Amazon S3 bucket, an Lambda function, or an Amazon Machine Image (AMI) based on Amazon EC2 that is associated with a particular job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Resources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ResourceList\"\n        },\n        {\n          \"description\": \"An array of <code>S3Resource</code> objects.\"\n        }\n      ]\n    },\n    \"LambdaResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaResourceList\"\n        },\n        {\n          \"description\": \"The Python-language Lambda\
  \ functions for this job.\"\n        }\n      ]\n    },\n    \"Ec2AmiResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ec2AmiResourceList\"\n        },\n        {\n          \"description\": \"The Amazon Machine Images (AMIs) associated with this job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-job-resource-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: JobResource
---
