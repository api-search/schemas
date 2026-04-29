---
description: GetAllowListResponse schema from Amazon Macie API
layout: schema
name: GetAllowListResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: criteria
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: updatedAt
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-allow-list-response-schema.json
slug: amazon-macie-get-allow-list-response
source_filename: amazon-macie-get-allow-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-allow-list-response-schema.json\",\n  \"title\": \"GetAllowListResponse\",\n  \"description\": \"GetAllowListResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin71Max89PatternArnAwsAwsCnAwsUsGovMacie2AZ19920D12AllowListAZ0922\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the allow list.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the allow list was created in Amazon Macie.\"\n        }\n      ]\n \
  \   },\n    \"criteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowListCriteria\"\n        },\n        {\n          \"description\": \"The criteria that specify the text or text pattern to ignore. The criteria can be the location and name of an S3 object that lists specific text to ignore (s3WordsList), or a regular expression (regex) that defines a text pattern to ignore.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max512PatternSS\"\n        },\n        {\n          \"description\": \"The custom description of the allow list.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin22Max22PatternAZ0922\"\n        },\n        {\n          \"description\": \"The unique identifier for the allow list.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/__stringMin1Max128Pattern\"\n        },\n        {\n          \"description\": \"The custom name of the allow list.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowListStatus\"\n        },\n        {\n          \"description\": \"The current status of the allow list, which indicates whether Amazon Macie can access and use the list's criteria.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map of key-value pairs that specifies which tags (keys and values) are associated with the allow list.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO\
  \ 8601 format, when the allow list's settings were most recently changed in Amazon Macie.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-allow-list-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetAllowListResponse
---
