---
description: Input to the <code>MergeDeveloperIdentities</code> action.
layout: schema
name: MergeDeveloperIdentitiesInput
properties_list:
- description: ''
  name: SourceUserIdentifier
  type: object
- description: ''
  name: DestinationUserIdentifier
  type: object
- description: ''
  name: DeveloperProviderName
  type: object
- description: ''
  name: IdentityPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-merge-developer-identities-input-schema.json
slug: identity-pools-merge-developer-identities-input
source_filename: identity-pools-merge-developer-identities-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-merge-developer-identities-input-schema.json\",\n  \"title\": \"MergeDeveloperIdentitiesInput\",\n  \"description\": \"Input to the <code>MergeDeveloperIdentities</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceUserIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeveloperUserIdentifier\"\n        },\n        {\n          \"description\": \"User identifier for the source user. The value should be a <code>DeveloperUserIdentifier</code>.\"\n        }\n      ]\n    },\n    \"DestinationUserIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeveloperUserIdentifier\"\n        },\n        {\n          \"description\": \"User identifier for the destination user. The value should be a <code>DeveloperUserIdentifier</code>.\"\
  \n        }\n      ]\n    },\n    \"DeveloperProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeveloperProviderName\"\n        },\n        {\n          \"description\": \"The \\\"domain\\\" by which Cognito will refer to your users. This is a (pseudo) domain name that you provide while creating an identity pool. This name acts as a placeholder that allows your backend and the Cognito service to communicate about the developer provider. For the <code>DeveloperProviderName</code>, you can use letters as well as period (.), underscore (_), and dash (-).\"\n        }\n      ]\n    },\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SourceUserIdentifier\",\n    \"DestinationUserIdentifier\",\n    \"DeveloperProviderName\"\
  ,\n    \"IdentityPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-merge-developer-identities-input-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: MergeDeveloperIdentitiesInput
---
