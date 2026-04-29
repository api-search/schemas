---
description: SetRiskConfigurationRequest schema from Amazon Cognito
layout: schema
name: SetRiskConfigurationRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: ClientId
  type: object
- description: ''
  name: CompromisedCredentialsRiskConfiguration
  type: object
- description: ''
  name: AccountTakeoverRiskConfiguration
  type: object
- description: ''
  name: RiskExceptionConfiguration
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-set-risk-configuration-request-schema.json
slug: cognito-idp-set-risk-configuration-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID. \"\n        }\n      ]\n    },\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientIdType\"\n        },\n        {\n          \"description\": \"<p>The app client ID. If <code>ClientId</code> is null, then the risk configuration is mapped to <code>userPoolId</code>. When the client ID is null, the same risk configuration is applied to all the clients in the userPool.</p> <p>Otherwise, <code>ClientId</code> is mapped to the client. When the client ID isn't null, the user pool configuration is overridden and the risk configuration for the client is used instead.</p>\"\n        }\n      ]\n    },\n    \"CompromisedCredentialsRiskConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/CompromisedCredentialsRiskConfigurationType\"\n        },\n        {\n          \"description\": \"The compromised credentials risk configuration.\"\n        }\n      ]\n    },\n    \"AccountTakeoverRiskConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountTakeoverRiskConfigurationType\"\n        },\n        {\n          \"description\": \"The account takeover risk configuration.\"\n        }\n      ]\n    },\n    \"RiskExceptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RiskExceptionConfigurationType\"\n        },\n        {\n          \"description\": \"The configuration to override the risk decision.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-set-risk-configuration-request-schema.json\"\
  ,\n  \"title\": \"SetRiskConfigurationRequest\",\n  \"description\": \"SetRiskConfigurationRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-set-risk-configuration-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: SetRiskConfigurationRequest
---
