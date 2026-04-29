---
description: A user profile in a Amazon Cognito user pool.
layout: schema
name: UserType
properties_list:
- description: ''
  name: Username
  type: object
- description: ''
  name: Attributes
  type: object
- description: ''
  name: UserCreateDate
  type: object
- description: ''
  name: UserLastModifiedDate
  type: object
- description: ''
  name: Enabled
  type: object
- description: ''
  name: UserStatus
  type: object
- description: ''
  name: MFAOptions
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-user-type-schema.json
slug: cognito-idp-user-type
source_filename: cognito-idp-user-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The user name of the user you want to describe.\"\n        }\n      ]\n    },\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeListType\"\n        },\n        {\n          \"description\": \"A container with information about the user type attributes.\"\n        }\n      ]\n    },\n    \"UserCreateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The creation date of the user.\"\n        }\n      ]\n    },\n    \"UserLastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The last modified date of the user.\"\
  \n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"Specifies whether the user is enabled.\"\n        }\n      ]\n    },\n    \"UserStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserStatusType\"\n        },\n        {\n          \"description\": \"<p>The user status. This can be one of the following:</p> <ul> <li> <p>UNCONFIRMED - User has been created but not confirmed.</p> </li> <li> <p>CONFIRMED - User has been confirmed.</p> </li> <li> <p>EXTERNAL_PROVIDER - User signed in with a third-party IdP.</p> </li> <li> <p>ARCHIVED - User is no longer active.</p> </li> <li> <p>UNKNOWN - User status isn't known.</p> </li> <li> <p>RESET_REQUIRED - User is confirmed, but the user must request a code and reset their password before they can sign in.</p> </li> <li> <p>FORCE_CHANGE_PASSWORD - The user is confirmed and the\
  \ user can sign in using a temporary password, but on first sign-in, the user must change their password to a new value before doing anything else. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"MFAOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MFAOptionListType\"\n        },\n        {\n          \"description\": \"The MFA options for the user.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A user profile in a Amazon Cognito user pool.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-user-type-schema.json\",\n  \"title\": \"UserType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-user-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UserType
---
