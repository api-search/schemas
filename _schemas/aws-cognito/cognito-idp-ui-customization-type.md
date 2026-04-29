---
description: A container for the UI customization information for a user pool's built-in app UI.
layout: schema
name: UICustomizationType
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: ClientId
  type: object
- description: ''
  name: ImageUrl
  type: object
- description: ''
  name: CSS
  type: object
- description: ''
  name: CSSVersion
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: CreationDate
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-ui-customization-type-schema.json
slug: cognito-idp-ui-customization-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientIdType\"\n        },\n        {\n          \"description\": \"The client ID for the client app.\"\n        }\n      ]\n    },\n    \"ImageUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageUrlType\"\n        },\n        {\n          \"description\": \"The logo image for the UI customization.\"\n        }\n      ]\n    },\n    \"CSS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CSSType\"\n        },\n        {\n          \"description\": \"The CSS values in the UI customization.\"\n        }\n      ]\n    },\n    \"CSSVersion\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CSSVersionType\"\n        },\n        {\n          \"description\": \"The CSS version number.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The last-modified date for the UI customization.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The creation date for the UI customization.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A container for the UI customization information for a user pool's built-in app UI.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-ui-customization-type-schema.json\"\
  ,\n  \"title\": \"UICustomizationType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-ui-customization-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UICustomizationType
---
