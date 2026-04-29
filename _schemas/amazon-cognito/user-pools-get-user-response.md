---
description: Represents the response from the server from the request to get information about the user.
layout: schema
name: GetUserResponse
properties_list:
- description: ''
  name: Username
  type: object
- description: ''
  name: UserAttributes
  type: object
- description: ''
  name: MFAOptions
  type: object
- description: ''
  name: PreferredMfaSetting
  type: object
- description: ''
  name: UserMFASettingList
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-user-response-schema.json
slug: user-pools-get-user-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-user-response-schema.json\",\n  \"title\": \"GetUserResponse\",\n  \"description\": \"Represents the response from the server from the request to get information about the user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The username of the user that you requested.\"\n        }\n      ]\n    },\n    \"UserAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeListType\"\n        },\n        {\n          \"description\": \"<p>An array of name-value pairs representing user attributes.</p> <p>For custom attributes, you must prepend the <code>custom:</code> prefix to the attribute\
  \ name.</p>\"\n        }\n      ]\n    },\n    \"MFAOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MFAOptionListType\"\n        },\n        {\n          \"description\": \" <i>This response parameter is no longer supported.</i> It provides information only about SMS MFA configurations. It doesn't provide information about time-based one-time password (TOTP) software token MFA configurations. To look up information about either type of MFA configuration, use UserMFASettingList instead.\"\n        }\n      ]\n    },\n    \"PreferredMfaSetting\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The user's preferred MFA setting.\"\n        }\n      ]\n    },\n    \"UserMFASettingList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserMFASettingListType\"\n        },\n        {\n          \"description\": \"The MFA options that\
  \ are activated for the user. The possible values in this list are <code>SMS_MFA</code> and <code>SOFTWARE_TOKEN_MFA</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Username\",\n    \"UserAttributes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-user-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: GetUserResponse
---
