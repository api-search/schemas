---
description: GetFindingsResponse schema from Amazon Macie API
layout: schema
name: GetFindingsResponse
properties_list:
- description: ''
  name: findings
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-findings-response-schema.json
slug: amazon-macie-get-findings-response
source_filename: amazon-macie-get-findings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-findings-response-schema.json\",\n  \"title\": \"GetFindingsResponse\",\n  \"description\": \"GetFindingsResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfFinding\"\n        },\n        {\n          \"description\": \"An array of objects, one for each finding that matches the criteria specified in the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-findings-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetFindingsResponse
---
