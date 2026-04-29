---
description: The request to respond to the authentication challenge, as an administrator.
layout: schema
name: AdminRespondToAuthChallengeRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: ClientId
  type: object
- description: ''
  name: ChallengeName
  type: object
- description: ''
  name: ChallengeResponses
  type: object
- description: ''
  name: Session
  type: object
- description: ''
  name: AnalyticsMetadata
  type: object
- description: ''
  name: ContextData
  type: object
- description: ''
  name: ClientMetadata
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-admin-respond-to-auth-challenge-request-schema.json
slug: cognito-idp-admin-respond-to-auth-challenge-request
source_filename: cognito-idp-admin-respond-to-auth-challenge-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Cognito user pool.\"\n        }\n      ]\n    },\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientIdType\"\n        },\n        {\n          \"description\": \"The app client ID.\"\n        }\n      ]\n    },\n    \"ChallengeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChallengeNameType\"\n        },\n        {\n          \"description\": \"The challenge name. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_AdminInitiateAuth.html\\\">AdminInitiateAuth</a>.\"\n        }\n      ]\n    },\n    \"ChallengeResponses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChallengeResponsesType\"\
  \n        },\n        {\n          \"description\": \"<p>The challenge responses. These are inputs corresponding to the value of <code>ChallengeName</code>, for example:</p> <ul> <li> <p> <code>SMS_MFA</code>: <code>SMS_MFA_CODE</code>, <code>USERNAME</code>, <code>SECRET_HASH</code> (if app client is configured with client secret).</p> </li> <li> <p> <code>PASSWORD_VERIFIER</code>: <code>PASSWORD_CLAIM_SIGNATURE</code>, <code>PASSWORD_CLAIM_SECRET_BLOCK</code>, <code>TIMESTAMP</code>, <code>USERNAME</code>, <code>SECRET_HASH</code> (if app client is configured with client secret).</p> <note> <p> <code>PASSWORD_VERIFIER</code> requires <code>DEVICE_KEY</code> when signing in with a remembered device.</p> </note> </li> <li> <p> <code>ADMIN_NO_SRP_AUTH</code>: <code>PASSWORD</code>, <code>USERNAME</code>, <code>SECRET_HASH</code> (if app client is configured with client secret). </p> </li> <li> <p> <code>NEW_PASSWORD_REQUIRED</code>: <code>NEW_PASSWORD</code>, <code>USERNAME</code>, <code>SECRET_HASH</code>\
  \ (if app client is configured with client secret). To set any required attributes that Amazon Cognito returned as <code>requiredAttributes</code> in the <code>AdminInitiateAuth</code> response, add a <code>userAttributes.<i>attributename</i> </code> parameter. This parameter can also set values for writable attributes that aren't required by your user pool.</p> <note> <p>In a <code>NEW_PASSWORD_REQUIRED</code> challenge response, you can't modify a required attribute that already has a value. In <code>AdminRespondToAuthChallenge</code>, set a value for any keys that Amazon Cognito returned in the <code>requiredAttributes</code> parameter, then use the <code>AdminUpdateUserAttributes</code> API operation to modify the value of any additional attributes.</p> </note> </li> <li> <p> <code>MFA_SETUP</code> requires <code>USERNAME</code>, plus you must use the session value returned by <code>VerifySoftwareToken</code> in the <code>Session</code> parameter.</p> </li> </ul> <p>The value of the\
  \ <code>USERNAME</code> attribute must be the user's actual username, not an alias (such as an email address or phone number). To make this simpler, the <code>AdminInitiateAuth</code> response includes the actual username value in the <code>USERNAMEUSER_ID_FOR_SRP</code> attribute. This happens even if you specified an alias in your call to <code>AdminInitiateAuth</code>.</p>\"\n        }\n      ]\n    },\n    \"Session\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionType\"\n        },\n        {\n          \"description\": \"The session that should be passed both ways in challenge-response calls to the service. If an <code>InitiateAuth</code> or <code>RespondToAuthChallenge</code> API call determines that the caller must pass another challenge, it returns a session with other challenge parameters. This session should be passed as it is to the next <code>RespondToAuthChallenge</code> API call.\"\n        }\n      ]\n    },\n    \"AnalyticsMetadata\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyticsMetadataType\"\n        },\n        {\n          \"description\": \"The analytics metadata for collecting Amazon Pinpoint metrics for <code>AdminRespondToAuthChallenge</code> calls.\"\n        }\n      ]\n    },\n    \"ContextData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContextDataType\"\n        },\n        {\n          \"description\": \"Contextual data about your user session, such as the device fingerprint, IP address, or location. Amazon Cognito advanced security evaluates the risk of an authentication event based on the context that your app generates and passes to Amazon Cognito when it makes API requests.\"\n        }\n      ]\n    },\n    \"ClientMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientMetadataType\"\n        },\n        {\n          \"description\": \"<p>A map of custom key-value pairs that you can\
  \ provide as input for any custom workflows that this action triggers.</p> <p>You create custom workflows by assigning Lambda functions to user pool triggers. When you use the AdminRespondToAuthChallenge API action, Amazon Cognito invokes any functions that you have assigned to the following triggers: </p> <ul> <li> <p>pre sign-up</p> </li> <li> <p>custom message</p> </li> <li> <p>post authentication</p> </li> <li> <p>user migration</p> </li> <li> <p>pre token generation</p> </li> <li> <p>define auth challenge</p> </li> <li> <p>create auth challenge</p> </li> <li> <p>verify auth challenge response</p> </li> </ul> <p>When Amazon Cognito invokes any of these functions, it passes a JSON payload, which the function receives as input. This payload contains a <code>clientMetadata</code> attribute that provides the data that you assigned to the ClientMetadata parameter in your AdminRespondToAuthChallenge request. In your function code in Lambda, you can process the <code>clientMetadata</code>\
  \ value to enhance your workflow for your specific needs.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-identity-pools-working-with-aws-lambda-triggers.html\\\"> Customizing user pool Workflows with Lambda Triggers</a> in the <i>Amazon Cognito Developer Guide</i>.</p> <note> <p>When you use the ClientMetadata parameter, remember that Amazon Cognito won't do the following:</p> <ul> <li> <p>Store the ClientMetadata value. This data is available only to Lambda triggers that are assigned to a user pool to support custom workflows. If your user pool configuration doesn't include triggers, the ClientMetadata parameter serves no purpose.</p> </li> <li> <p>Validate the ClientMetadata value.</p> </li> <li> <p>Encrypt the ClientMetadata value. Don't use Amazon Cognito to provide sensitive information.</p> </li> </ul> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"ClientId\",\n    \"ChallengeName\"\
  \n  ],\n  \"description\": \"The request to respond to the authentication challenge, as an administrator.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-respond-to-auth-challenge-request-schema.json\",\n  \"title\": \"AdminRespondToAuthChallengeRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-respond-to-auth-challenge-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AdminRespondToAuthChallengeRequest
---
