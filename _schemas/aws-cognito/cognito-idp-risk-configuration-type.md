---
description: The risk configuration type.
layout: schema
name: RiskConfigurationType
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
- description: ''
  name: LastModifiedDate
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-risk-configuration-type-schema.json
slug: cognito-idp-risk-configuration-type
source_filename: cognito-idp-risk-configuration-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientIdType\"\n        },\n        {\n          \"description\": \"The app client ID.\"\n        }\n      ]\n    },\n    \"CompromisedCredentialsRiskConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompromisedCredentialsRiskConfigurationType\"\n        },\n        {\n          \"description\": \"The compromised credentials risk configuration object, including the <code>EventFilter</code> and the <code>EventAction</code>.\"\n        }\n      ]\n    },\n    \"AccountTakeoverRiskConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountTakeoverRiskConfigurationType\"\
  \n        },\n        {\n          \"description\": \"The account takeover risk configuration object, including the <code>NotifyConfiguration</code> object and <code>Actions</code> to take if there is an account takeover.\"\n        }\n      ]\n    },\n    \"RiskExceptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RiskExceptionConfigurationType\"\n        },\n        {\n          \"description\": \"The configuration to override the risk decision.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The last modified date.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The risk configuration type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-risk-configuration-type-schema.json\"\
  ,\n  \"title\": \"RiskConfigurationType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-risk-configuration-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: RiskConfigurationType
---
