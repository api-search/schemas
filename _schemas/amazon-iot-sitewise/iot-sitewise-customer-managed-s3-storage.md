---
description: Contains information about a customer managed Amazon S3 bucket.
layout: schema
name: CustomerManagedS3Storage
properties_list:
- description: ''
  name: s3ResourceArn
  type: object
- description: ''
  name: roleArn
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-customer-managed-s3-storage-schema.json
slug: iot-sitewise-customer-managed-s3-storage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-customer-managed-s3-storage-schema.json\",\n  \"title\": \"CustomerManagedS3Storage\",\n  \"description\": \"Contains information about a customer managed Amazon S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the Amazon S3 object. For more information about how to find the ARN for an Amazon S3 object, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/s3-arn-format.html\\\">Amazon S3 resources</a> in the <i>Amazon Simple Storage Service User Guide</i>.\"\n        }\n      ]\n    },\n    \"roleArn\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the Identity and Access Management role that allows IoT SiteWise to send data to Amazon S3.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"s3ResourceArn\",\n    \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-customer-managed-s3-storage-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: CustomerManagedS3Storage
---
