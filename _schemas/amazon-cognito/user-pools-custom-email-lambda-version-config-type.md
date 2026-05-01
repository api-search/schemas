---
description: A custom email sender Lambda configuration type.
layout: schema
name: CustomEmailLambdaVersionConfigType
properties_list:
- description: ''
  name: LambdaVersion
  type: object
- description: ''
  name: LambdaArn
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-custom-email-lambda-version-config-type-schema.json
slug: user-pools-custom-email-lambda-version-config-type
source_filename: user-pools-custom-email-lambda-version-config-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-custom-email-lambda-version-config-type-schema.json\",\n  \"title\": \"CustomEmailLambdaVersionConfigType\",\n  \"description\": \"A custom email sender Lambda configuration type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LambdaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomEmailSenderLambdaVersionType\"\n        },\n        {\n          \"description\": \"Signature of the \\\"request\\\" attribute in the \\\"event\\\" information Amazon Cognito passes to your custom email Lambda function. The only supported value is <code>V1_0</code>.\"\n        }\n      ]\n    },\n    \"LambdaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The Amazon\
  \ Resource Name (ARN) of the Lambda function that Amazon Cognito activates to send email notifications to users.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LambdaVersion\",\n    \"LambdaArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-custom-email-lambda-version-config-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: CustomEmailLambdaVersionConfigType
---
