---
description: ListSensitivityInspectionTemplatesResponse schema from Amazon Macie API
layout: schema
name: ListSensitivityInspectionTemplatesResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: sensitivityInspectionTemplates
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-list-sensitivity-inspection-templates-response-schema.json
slug: amazon-macie-list-sensitivity-inspection-templates-response
source_filename: amazon-macie-list-sensitivity-inspection-templates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-sensitivity-inspection-templates-response-schema.json\",\n  \"title\": \"ListSensitivityInspectionTemplatesResponse\",\n  \"description\": \"ListSensitivityInspectionTemplatesResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The string to use in a subsequent request to get the next page of results in a paginated response. This value is null if there are no additional pages.\"\n        }\n      ]\n    },\n    \"sensitivityInspectionTemplates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSensitivityInspectionTemplatesEntry\"\n        },\n        {\n    \
  \      \"description\": \"An array that specifies the unique identifier and name of the sensitivity inspection template for the account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-sensitivity-inspection-templates-response-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ListSensitivityInspectionTemplatesResponse
---
