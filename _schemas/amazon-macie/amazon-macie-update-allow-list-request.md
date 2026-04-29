---
description: UpdateAllowListRequest schema from Amazon Macie API
layout: schema
name: UpdateAllowListRequest
properties_list:
- description: ''
  name: criteria
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-update-allow-list-request-schema.json
slug: amazon-macie-update-allow-list-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-allow-list-request-schema.json\",\n  \"title\": \"UpdateAllowListRequest\",\n  \"description\": \"UpdateAllowListRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"criteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowListCriteria\"\n        },\n        {\n          \"description\": \"<p>The criteria that specify the text or text pattern to ignore. The criteria can be the location and name of an S3 object that lists specific text to ignore (s3WordsList), or a regular expression that defines a text pattern to ignore (regex).</p> <p>You can change a list's underlying criteria, such as the name of the S3 object or the regular expression to use. However, you can't change the type from s3WordsList to regex or\
  \ the other way around.</p>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max512PatternSS\"\n        },\n        {\n          \"description\": \"A custom description of the allow list. The description can contain as many as 512 characters.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max128Pattern\"\n        },\n        {\n          \"description\": \"A custom name for the allow list. The name can contain as many as 128 characters.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"criteria\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-allow-list-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UpdateAllowListRequest
---
