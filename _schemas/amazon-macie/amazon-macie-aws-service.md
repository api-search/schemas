---
description: Provides information about an Amazon Web Service that performed an action on an affected resource.
layout: schema
name: AwsService
properties_list:
- description: ''
  name: invokedBy
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-aws-service-schema.json
slug: amazon-macie-aws-service
source_filename: amazon-macie-aws-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-aws-service-schema.json\",\n  \"title\": \"AwsService\",\n  \"description\": \"Provides information about an Amazon Web Service that performed an action on an affected resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invokedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the Amazon Web Service that performed the action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-aws-service-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: AwsService
---
