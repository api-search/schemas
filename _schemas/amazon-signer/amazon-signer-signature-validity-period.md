---
description: The validity period for a signing job.
layout: schema
name: SignatureValidityPeriod
properties_list:
- description: ''
  name: value
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-signature-validity-period-schema.json
slug: amazon-signer-signature-validity-period
source_filename: amazon-signer-signature-validity-period-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signature-validity-period-schema.json\",\n  \"title\": \"SignatureValidityPeriod\",\n  \"description\": \"The validity period for a signing job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"allOf\": [\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"description\": \"The numerical value of the time unit for signature validity.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"DAYS\",\n            \"MONTHS\",\n            \"YEARS\"\n          ]\n        },\n        {\n          \"description\": \"The time unit for signature validity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signature-validity-period-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: SignatureValidityPeriod
---
