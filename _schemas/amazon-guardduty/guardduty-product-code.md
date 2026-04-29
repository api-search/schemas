---
description: Contains information about the product code for the EC2 instance.
layout: schema
name: ProductCode
properties_list:
- description: ''
  name: Code
  type: object
- description: ''
  name: ProductType
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-product-code-schema.json
slug: guardduty-product-code
source_filename: guardduty-product-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-product-code-schema.json\",\n  \"title\": \"ProductCode\",\n  \"description\": \"Contains information about the product code for the EC2 instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"productCodeId\"\n          },\n          \"description\": \"The product code information.\"\n        }\n      ]\n    },\n    \"ProductType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"productCodeType\"\n          },\n          \"description\": \"The product code type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-product-code-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ProductCode
---
