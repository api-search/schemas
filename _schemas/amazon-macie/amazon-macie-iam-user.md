---
description: Provides information about an Identity and Access Management (IAM) user who performed an action on an affected resource.
layout: schema
name: IamUser
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: principalId
  type: object
- description: ''
  name: userName
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-iam-user-schema.json
slug: amazon-macie-iam-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-iam-user-schema.json\",\n  \"title\": \"IamUser\",\n  \"description\": \"Provides information about an Identity and Access Management (IAM) user who performed an action on an affected resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the Amazon Web Services account that's associated with the IAM user who performed the action.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the principal that performed the action. The last section of\
  \ the ARN contains the name of the user who performed the action.\"\n        }\n      ]\n    },\n    \"principalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the IAM user who performed the action.\"\n        }\n      ]\n    },\n    \"userName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The username of the IAM user who performed the action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-iam-user-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: IamUser
---
