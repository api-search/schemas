---
description: CreateAllowListRequest schema from Amazon Macie API
layout: schema
name: CreateAllowListRequest
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: criteria
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-create-allow-list-request-schema.json
slug: amazon-macie-create-allow-list-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-allow-list-request-schema.json\",\n  \"title\": \"CreateAllowListRequest\",\n  \"description\": \"CreateAllowListRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive token that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"criteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowListCriteria\"\n        },\n        {\n          \"description\": \"The criteria that specify the text or text pattern to ignore. The criteria can be the location and name of an S3 object that lists specific text\
  \ to ignore (s3WordsList), or a regular expression (regex) that defines a text pattern to ignore.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max512PatternSS\"\n        },\n        {\n          \"description\": \"A custom description of the allow list. The description can contain as many as 512 characters.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max128Pattern\"\n        },\n        {\n          \"description\": \"A custom name for the allow list. The name can contain as many as 128 characters.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"<p>A map of key-value pairs that specifies the tags to associate with the allow list.</p> <p>An allow list can have a maximum\
  \ of 50 tags. Each tag consists of a tag key and an associated tag value. The maximum length of a tag key is 128 characters. The maximum length of a tag value is 256 characters.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"criteria\",\n    \"clientToken\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-allow-list-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CreateAllowListRequest
---
