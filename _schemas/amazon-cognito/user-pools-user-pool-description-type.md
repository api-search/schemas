---
description: A user pool description.
layout: schema
name: UserPoolDescriptionType
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: LambdaConfig
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: CreationDate
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-user-pool-description-type-schema.json
slug: user-pools-user-pool-description-type
source_filename: user-pools-user-pool-description-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-pool-description-type-schema.json\",\n  \"title\": \"UserPoolDescriptionType\",\n  \"description\": \"A user pool description.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The ID in a user pool description.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolNameType\"\n        },\n        {\n          \"description\": \"The name in a user pool description.\"\n        }\n      ]\n    },\n    \"LambdaConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaConfigType\"\n        },\n        {\n          \"description\"\
  : \"The Lambda configuration information in a user pool description.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusType\"\n        },\n        {\n          \"description\": \"The user pool status in a user pool description.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601</a> format, when the item was modified.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601</a> format, when the item was created.\"\n        }\n  \
  \    ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-pool-description-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: UserPoolDescriptionType
---
