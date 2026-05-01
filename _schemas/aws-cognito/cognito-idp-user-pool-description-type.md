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
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-user-pool-description-type-schema.json
slug: cognito-idp-user-pool-description-type
source_filename: cognito-idp-user-pool-description-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The ID in a user pool description.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolNameType\"\n        },\n        {\n          \"description\": \"The name in a user pool description.\"\n        }\n      ]\n    },\n    \"LambdaConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaConfigType\"\n        },\n        {\n          \"description\": \"The Lambda configuration information in a user pool description.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusType\"\n        },\n        {\n          \"description\": \"The user pool status in a user pool description.\"\n    \
  \    }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date the user pool description was last modified.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date the user pool description was created.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A user pool description.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-user-pool-description-type-schema.json\",\n  \"title\": \"UserPoolDescriptionType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-user-pool-description-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UserPoolDescriptionType
---
