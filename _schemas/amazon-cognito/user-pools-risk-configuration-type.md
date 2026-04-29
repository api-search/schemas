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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-risk-configuration-type-schema.json
slug: user-pools-risk-configuration-type
source_filename: user-pools-risk-configuration-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-risk-configuration-type-schema.json\",\n  \"title\": \"RiskConfigurationType\",\n  \"description\": \"The risk configuration type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientIdType\"\n        },\n        {\n          \"description\": \"The app client ID.\"\n        }\n      ]\n    },\n    \"CompromisedCredentialsRiskConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompromisedCredentialsRiskConfigurationType\"\n        },\n       \
  \ {\n          \"description\": \"The compromised credentials risk configuration object, including the <code>EventFilter</code> and the <code>EventAction</code>.\"\n        }\n      ]\n    },\n    \"AccountTakeoverRiskConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountTakeoverRiskConfigurationType\"\n        },\n        {\n          \"description\": \"The account takeover risk configuration object, including the <code>NotifyConfiguration</code> object and <code>Actions</code> to take if there is an account takeover.\"\n        }\n      ]\n    },\n    \"RiskExceptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RiskExceptionConfigurationType\"\n        },\n        {\n          \"description\": \"The configuration to override the risk decision.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n  \
  \      },\n        {\n          \"description\": \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601</a> format, when the item was modified.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-risk-configuration-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: RiskConfigurationType
---
