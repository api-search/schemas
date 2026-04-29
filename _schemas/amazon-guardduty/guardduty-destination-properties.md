---
description: Contains the Amazon Resource Name (ARN) of the resource to publish to, such as an S3 bucket, and the ARN of the KMS key to use to encrypt published findings.
layout: schema
name: DestinationProperties
properties_list:
- description: ''
  name: DestinationArn
  type: object
- description: ''
  name: KmsKeyArn
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-destination-properties-schema.json
slug: guardduty-destination-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-destination-properties-schema.json\",\n  \"title\": \"DestinationProperties\",\n  \"description\": \"Contains the Amazon Resource Name (ARN) of the resource to publish to, such as an S3 bucket, and the ARN of the KMS key to use to encrypt published findings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationArn\"\n          },\n          \"description\": \"<p>The ARN of the resource to publish to.</p> <p>To specify an S3 bucket folder use the following format: <code>arn:aws:s3:::DOC-EXAMPLE-BUCKET/myFolder/</code> </p>\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kmsKeyArn\"\n          },\n          \"description\": \"The ARN of the KMS key to use for encryption.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-destination-properties-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DestinationProperties
---
