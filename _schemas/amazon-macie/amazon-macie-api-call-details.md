---
description: Provides information about an API operation that an entity invoked for an affected resource.
layout: schema
name: ApiCallDetails
properties_list:
- description: ''
  name: api
  type: object
- description: ''
  name: apiServiceName
  type: object
- description: ''
  name: firstSeen
  type: object
- description: ''
  name: lastSeen
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-api-call-details-schema.json
slug: amazon-macie-api-call-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-api-call-details-schema.json\",\n  \"title\": \"ApiCallDetails\",\n  \"description\": \"Provides information about an API operation that an entity invoked for an affected resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the operation that was invoked most recently and produced the finding.\"\n        }\n      ]\n    },\n    \"apiServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL of the Amazon Web Service that provides the operation, for example: s3.amazonaws.com.\"\n        }\n      ]\n    },\n    \"firstSeen\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The first date and time, in UTC and extended ISO 8601 format, when any operation was invoked and produced the finding.\"\n        }\n      ]\n    },\n    \"lastSeen\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The most recent date and time, in UTC and extended ISO 8601 format, when the specified operation (api) was invoked and produced the finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-api-call-details-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ApiCallDetails
---
