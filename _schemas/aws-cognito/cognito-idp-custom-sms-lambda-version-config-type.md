---
description: A custom SMS sender Lambda configuration type.
layout: schema
name: CustomSMSLambdaVersionConfigType
properties_list:
- description: ''
  name: LambdaVersion
  type: object
- description: ''
  name: LambdaArn
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-custom-sms-lambda-version-config-type-schema.json
slug: cognito-idp-custom-sms-lambda-version-config-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LambdaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomSMSSenderLambdaVersionType\"\n        },\n        {\n          \"description\": \"Signature of the \\\"request\\\" attribute in the \\\"event\\\" information that Amazon Cognito passes to your custom SMS Lambda function. The only supported value is <code>V1_0</code>.\"\n        }\n      ]\n    },\n    \"LambdaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Lambda function that Amazon Cognito activates to send SMS notifications to users.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LambdaVersion\",\n    \"LambdaArn\"\n  ],\n  \"description\": \"A custom SMS sender Lambda configuration type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"\
  https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-custom-sms-lambda-version-config-type-schema.json\",\n  \"title\": \"CustomSMSLambdaVersionConfigType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-custom-sms-lambda-version-config-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: CustomSMSLambdaVersionConfigType
---
