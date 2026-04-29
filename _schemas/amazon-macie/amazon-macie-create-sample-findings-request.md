---
description: CreateSampleFindingsRequest schema from Amazon Macie API
layout: schema
name: CreateSampleFindingsRequest
properties_list:
- description: ''
  name: findingTypes
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-create-sample-findings-request-schema.json
slug: amazon-macie-create-sample-findings-request
source_filename: amazon-macie-create-sample-findings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-sample-findings-request-schema.json\",\n  \"title\": \"CreateSampleFindingsRequest\",\n  \"description\": \"CreateSampleFindingsRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfFindingType\"\n        },\n        {\n          \"description\": \"An array of finding types, one for each type of sample finding to create. To create a sample of every type of finding that Amazon Macie supports, don't include this array in your request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-sample-findings-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CreateSampleFindingsRequest
---
