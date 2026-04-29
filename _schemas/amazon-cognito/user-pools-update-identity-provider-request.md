---
description: UpdateIdentityProviderRequest schema from Amazon Cognito API
layout: schema
name: UpdateIdentityProviderRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: ProviderName
  type: object
- description: ''
  name: ProviderDetails
  type: object
- description: ''
  name: AttributeMapping
  type: object
- description: ''
  name: IdpIdentifiers
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-update-identity-provider-request-schema.json
slug: user-pools-update-identity-provider-request
source_filename: user-pools-update-identity-provider-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-identity-provider-request-schema.json\",\n  \"title\": \"UpdateIdentityProviderRequest\",\n  \"description\": \"UpdateIdentityProviderRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"ProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderNameType\"\n        },\n        {\n          \"description\": \"The IdP name.\"\n        }\n      ]\n    },\n    \"ProviderDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderDetailsType\"\n        },\n   \
  \     {\n          \"description\": \"The IdP details to be updated, such as <code>MetadataURL</code> and <code>MetadataFile</code>.\"\n        }\n      ]\n    },\n    \"AttributeMapping\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeMappingType\"\n        },\n        {\n          \"description\": \"The IdP attribute mapping to be changed.\"\n        }\n      ]\n    },\n    \"IdpIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdpIdentifiersListType\"\n        },\n        {\n          \"description\": \"A list of IdP identifiers.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"ProviderName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-identity-provider-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UpdateIdentityProviderRequest
---
