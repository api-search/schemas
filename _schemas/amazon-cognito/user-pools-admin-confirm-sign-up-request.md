---
description: Confirm a user's registration as a user pool administrator.
layout: schema
name: AdminConfirmSignUpRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Username
  type: object
- description: ''
  name: ClientMetadata
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-admin-confirm-sign-up-request-schema.json
slug: user-pools-admin-confirm-sign-up-request
source_filename: user-pools-admin-confirm-sign-up-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-confirm-sign-up-request-schema.json\",\n  \"title\": \"AdminConfirmSignUpRequest\",\n  \"description\": \"Confirm a user's registration as a user pool administrator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for which you want to confirm user registration.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The user name for which you want to confirm user registration.\"\n        }\n      ]\n    },\n    \"ClientMetadata\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/ClientMetadataType\"\n        },\n        {\n          \"description\": \"<p>A map of custom key-value pairs that you can provide as input for any custom workflows that this action triggers.</p> <p>If your user pool configuration includes triggers, the AdminConfirmSignUp API action invokes the Lambda function that is specified for the <i>post confirmation</i> trigger. When Amazon Cognito invokes this function, it passes a JSON payload, which the function receives as input. In this payload, the <code>clientMetadata</code> attribute provides the data that you assigned to the ClientMetadata parameter in your AdminConfirmSignUp request. In your function code in Lambda, you can process the ClientMetadata value to enhance your workflow for your specific needs.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-identity-pools-working-with-aws-lambda-triggers.html\\\"> Customizing user pool\
  \ Workflows with Lambda Triggers</a> in the <i>Amazon Cognito Developer Guide</i>.</p> <note> <p>When you use the ClientMetadata parameter, remember that Amazon Cognito won't do the following:</p> <ul> <li> <p>Store the ClientMetadata value. This data is available only to Lambda triggers that are assigned to a user pool to support custom workflows. If your user pool configuration doesn't include triggers, the ClientMetadata parameter serves no purpose.</p> </li> <li> <p>Validate the ClientMetadata value.</p> </li> <li> <p>Encrypt the ClientMetadata value. Don't use Amazon Cognito to provide sensitive information.</p> </li> </ul> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"Username\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-confirm-sign-up-request-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: AdminConfirmSignUpRequest
---
