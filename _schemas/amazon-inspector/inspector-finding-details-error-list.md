---
description: FindingDetailsErrorList schema
layout: schema
name: FindingDetailsErrorList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-finding-details-error-list-schema.json
slug: inspector-finding-details-error-list
source_filename: inspector-finding-details-error-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-finding-details-error-list-schema.json\",\n  \"title\": \"FindingDetailsErrorList\",\n  \"description\": \"FindingDetailsErrorList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"errorCode\",\n      \"errorMessage\",\n      \"findingArn\"\n    ],\n    \"properties\": {\n      \"errorCode\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FindingDetailsErrorCode\"\n          },\n          {\n            \"description\": \"The error code.\"\n          }\n        ]\n      },\n      \"errorMessage\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"The error message.\"\n          }\n        ]\n\
  \      },\n      \"findingArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FindingArn\"\n          },\n          {\n            \"description\": \"The finding ARN that returned an error.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Details about an error encountered when trying to return vulnerability data for a finding.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-finding-details-error-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: FindingDetailsErrorList
---
