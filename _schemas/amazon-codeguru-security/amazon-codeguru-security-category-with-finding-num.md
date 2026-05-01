---
description: Information about a finding category with open findings.
layout: schema
name: CategoryWithFindingNum
properties_list:
- description: ''
  name: categoryName
  type: object
- description: ''
  name: findingNumber
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-category-with-finding-num-schema.json
slug: amazon-codeguru-security-category-with-finding-num
source_filename: amazon-codeguru-security-category-with-finding-num-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-category-with-finding-num-schema.json\",\n  \"title\": \"CategoryWithFindingNum\",\n  \"description\": \"Information about a finding category with open findings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"categoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the finding category. A finding category is determined by the detector that detected the finding.\"\n        }\n      ]\n    },\n    \"findingNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of open findings in the category.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-category-with-finding-num-schema.json
tags:
- Amazon
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: CategoryWithFindingNum
---
