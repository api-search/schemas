---
description: Provides information about an account that's associated with an Amazon Macie administrator account.
layout: schema
name: Member
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: administratorAccountId
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: email
  type: object
- description: ''
  name: invitedAt
  type: object
- description: ''
  name: masterAccountId
  type: object
- description: ''
  name: relationshipStatus
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: updatedAt
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-member-schema.json
slug: amazon-macie-member
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-member-schema.json\",\n  \"title\": \"Member\",\n  \"description\": \"Provides information about an account that's associated with an Amazon Macie administrator account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID for the account.\"\n        }\n      ]\n    },\n    \"administratorAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID for the administrator account.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the account.\"\n        }\n      ]\n    },\n    \"email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The email address for the account. This value is null if the account is associated with the administrator account through Organizations.\"\n        }\n      ]\n    },\n    \"invitedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when an Amazon Macie membership invitation was last sent to the account. This value is null if a Macie membership invitation hasn't been sent to the account.\"\n        }\n      ]\n    },\n    \"masterAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"(Deprecated) The Amazon Web Services account ID for the administrator account. This property has been replaced by the administratorAccountId property and is retained only for backward compatibility.\"\n        }\n      ]\n    },\n    \"relationshipStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelationshipStatus\"\n        },\n        {\n          \"description\": \"The current status of the relationship between the account and the administrator account.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map of key-value pairs that specifies which tags (keys and values) are associated with the account in Amazon Macie.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\
  \n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, of the most recent change to the status of the relationship between the account and the administrator account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-member-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: Member
---
