---
description: Specifies the configuration for Lambda triggers.
layout: schema
name: LambdaConfigType
properties_list:
- description: ''
  name: PreSignUp
  type: object
- description: ''
  name: CustomMessage
  type: object
- description: ''
  name: PostConfirmation
  type: object
- description: ''
  name: PreAuthentication
  type: object
- description: ''
  name: PostAuthentication
  type: object
- description: ''
  name: DefineAuthChallenge
  type: object
- description: ''
  name: CreateAuthChallenge
  type: object
- description: ''
  name: VerifyAuthChallengeResponse
  type: object
- description: ''
  name: PreTokenGeneration
  type: object
- description: ''
  name: UserMigration
  type: object
- description: ''
  name: CustomSMSSender
  type: object
- description: ''
  name: CustomEmailSender
  type: object
- description: ''
  name: KMSKeyID
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-lambda-config-type-schema.json
slug: cognito-idp-lambda-config-type
source_filename: cognito-idp-lambda-config-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"PreSignUp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"A pre-registration Lambda trigger.\"\n        }\n      ]\n    },\n    \"CustomMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"A custom Message Lambda trigger.\"\n        }\n      ]\n    },\n    \"PostConfirmation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"A post-confirmation Lambda trigger.\"\n        }\n      ]\n    },\n    \"PreAuthentication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"A pre-authentication Lambda trigger.\"\n        }\n      ]\n    },\n    \"PostAuthentication\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"A post-authentication Lambda trigger.\"\n        }\n      ]\n    },\n    \"DefineAuthChallenge\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"Defines the authentication challenge.\"\n        }\n      ]\n    },\n    \"CreateAuthChallenge\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"Creates an authentication challenge.\"\n        }\n      ]\n    },\n    \"VerifyAuthChallengeResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"Verifies the authentication challenge response.\"\n        }\n      ]\n    },\n    \"PreTokenGeneration\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"A Lambda trigger that is invoked before token generation.\"\n        }\n      ]\n    },\n    \"UserMigration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The user migration Lambda config type.\"\n        }\n      ]\n    },\n    \"CustomSMSSender\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomSMSLambdaVersionConfigType\"\n        },\n        {\n          \"description\": \"A custom SMS sender Lambda trigger.\"\n        }\n      ]\n    },\n    \"CustomEmailSender\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomEmailLambdaVersionConfigType\"\n        },\n        {\n          \"description\": \"A custom email sender Lambda trigger.\"\n        }\n      ]\n    },\n    \"KMSKeyID\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an <a href=\\\"/kms/latest/developerguide/concepts.html#master_keys\\\">KMS key</a>. Amazon Cognito uses the key to encrypt codes and temporary passwords sent to <code>CustomEmailSender</code> and <code>CustomSMSSender</code>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Specifies the configuration for Lambda triggers.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-lambda-config-type-schema.json\",\n  \"title\": \"LambdaConfigType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-lambda-config-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: LambdaConfigType
---
