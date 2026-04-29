---
description: Specifies the criteria for an allow list. The criteria must specify a regular expression (regex) or an S3 object (s3WordsList). It can't specify both.
layout: schema
name: AllowListCriteria
properties_list:
- description: ''
  name: regex
  type: object
- description: ''
  name: s3WordsList
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-allow-list-criteria-schema.json
slug: amazon-macie-allow-list-criteria
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-allow-list-criteria-schema.json\",\n  \"title\": \"AllowListCriteria\",\n  \"description\": \"Specifies the criteria for an allow list. The criteria must specify a regular expression (regex) or an S3 object (s3WordsList). It can't specify both.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"regex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max512PatternSS\"\n        },\n        {\n          \"description\": \"The regular expression (<i>regex</i>) that defines the text pattern to ignore. The expression can contain as many as 512 characters.\"\n        }\n      ]\n    },\n    \"s3WordsList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3WordsList\"\n        },\n        {\n          \"description\": \"The\
  \ location and name of the S3 object that lists specific text to ignore.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-allow-list-criteria-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: AllowListCriteria
---
