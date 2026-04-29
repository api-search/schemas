---
description: Specifies the location of an occurrence of sensitive data in an Adobe Portable Document Format file.
layout: schema
name: Page
properties_list:
- description: ''
  name: lineRange
  type: object
- description: ''
  name: offsetRange
  type: object
- description: ''
  name: pageNumber
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-page-schema.json
slug: amazon-macie-page
source_filename: amazon-macie-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-page-schema.json\",\n  \"title\": \"Page\",\n  \"description\": \"Specifies the location of an occurrence of sensitive data in an Adobe Portable Document Format file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Range\"\n        },\n        {\n          \"description\": \" <p>Reserved for future use.</p>\"\n        }\n      ]\n    },\n    \"offsetRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Range\"\n        },\n        {\n          \"description\": \" <p>Reserved for future use.</p>\"\n        }\n      ]\n    },\n    \"pageNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"\
  description\": \"The page number of the page that contains the sensitive data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-page-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: Page
---
