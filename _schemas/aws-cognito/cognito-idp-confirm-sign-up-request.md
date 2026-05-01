---
description: Represents the request to confirm registration of a user.
layout: schema
name: ConfirmSignUpRequest
properties_list:
- description: ''
  name: ClientId
  type: object
- description: ''
  name: SecretHash
  type: object
- description: ''
  name: Username
  type: object
- description: ''
  name: ConfirmationCode
  type: object
- description: ''
  name: ForceAliasCreation
  type: object
- description: ''
  name: AnalyticsMetadata
  type: object
- description: ''
  name: UserContextData
  type: object
- description: ''
  name: ClientMetadata
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-confirm-sign-up-request-schema.json
slug: cognito-idp-confirm-sign-up-request
source_filename: cognito-idp-confirm-sign-up-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientIdType\"\n        },\n        {\n          \"description\": \"The ID of the app client associated with the user pool.\"\n        }\n      ]\n    },\n    \"SecretHash\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretHashType\"\n        },\n        {\n          \"description\": \"A keyed-hash message authentication code (HMAC) calculated using the secret key of a user pool client and username plus the client ID in the message.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The user name of the user whose registration you want to confirm.\"\n        }\n      ]\n    },\n    \"ConfirmationCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/ConfirmationCodeType\"\n        },\n        {\n          \"description\": \"The confirmation code sent by a user's request to confirm registration.\"\n        }\n      ]\n    },\n    \"ForceAliasCreation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ForceAliasCreation\"\n        },\n        {\n          \"description\": \"Boolean to be specified to force user confirmation irrespective of existing alias. By default set to <code>False</code>. If this parameter is set to <code>True</code> and the phone number/email used for sign up confirmation already exists as an alias with a different user, the API call will migrate the alias from the previous user to the newly created user being confirmed. If set to <code>False</code>, the API will throw an <b>AliasExistsException</b> error.\"\n        }\n      ]\n    },\n    \"AnalyticsMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyticsMetadataType\"\
  \n        },\n        {\n          \"description\": \"The Amazon Pinpoint analytics metadata for collecting metrics for <code>ConfirmSignUp</code> calls.\"\n        }\n      ]\n    },\n    \"UserContextData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserContextDataType\"\n        },\n        {\n          \"description\": \"Contextual data about your user session, such as the device fingerprint, IP address, or location. Amazon Cognito advanced security evaluates the risk of an authentication event based on the context that your app generates and passes to Amazon Cognito when it makes API requests.\"\n        }\n      ]\n    },\n    \"ClientMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientMetadataType\"\n        },\n        {\n          \"description\": \"<p>A map of custom key-value pairs that you can provide as input for any custom workflows that this action triggers.</p> <p>You create custom workflows by\
  \ assigning Lambda functions to user pool triggers. When you use the ConfirmSignUp API action, Amazon Cognito invokes the function that is assigned to the <i>post confirmation</i> trigger. When Amazon Cognito invokes this function, it passes a JSON payload, which the function receives as input. This payload contains a <code>clientMetadata</code> attribute, which provides the data that you assigned to the ClientMetadata parameter in your ConfirmSignUp request. In your function code in Lambda, you can process the <code>clientMetadata</code> value to enhance your workflow for your specific needs.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-identity-pools-working-with-aws-lambda-triggers.html\\\"> Customizing user pool Workflows with Lambda Triggers</a> in the <i>Amazon Cognito Developer Guide</i>.</p> <note> <p>When you use the ClientMetadata parameter, remember that Amazon Cognito won't do the following:</p> <ul> <li>\
  \ <p>Store the ClientMetadata value. This data is available only to Lambda triggers that are assigned to a user pool to support custom workflows. If your user pool configuration doesn't include triggers, the ClientMetadata parameter serves no purpose.</p> </li> <li> <p>Validate the ClientMetadata value.</p> </li> <li> <p>Encrypt the ClientMetadata value. Don't use Amazon Cognito to provide sensitive information.</p> </li> </ul> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClientId\",\n    \"Username\",\n    \"ConfirmationCode\"\n  ],\n  \"description\": \"Represents the request to confirm registration of a user.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-confirm-sign-up-request-schema.json\",\n  \"title\": \"ConfirmSignUpRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-confirm-sign-up-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ConfirmSignUpRequest
---
