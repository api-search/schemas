---
description: Represents the response from the server from the request to get the specified user as an administrator.
layout: schema
name: AdminGetUserResponse
properties_list:
- description: ''
  name: Username
  type: object
- description: ''
  name: UserAttributes
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
- description: ''
  name: PreferredMfaSetting
  type: object
- description: ''
  name: UserMFASettingList
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-admin-get-user-response-schema.json
slug: user-pools-admin-get-user-response
source_filename: user-pools-admin-get-user-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-get-user-response-schema.json\",\n  \"title\": \"AdminGetUserResponse\",\n  \"description\": \"Represents the response from the server from the request to get the specified user as an administrator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The username of the user that you requested.\"\n        }\n      ]\n    },\n    \"UserAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeListType\"\n        },\n        {\n          \"description\": \"An array of name-value pairs representing user attributes.\"\n        }\n      ]\n    },\n    \"UserCreateDate\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date the user was created.\"\n        }\n      ]\n    },\n    \"UserLastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601</a> format, when the item was modified.\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"Indicates that the status is <code>enabled</code>.\"\n        }\n      ]\n    },\n    \"UserStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserStatusType\"\n        },\n        {\n          \"description\": \"<p>The user status. Can be one of the following:</p> <ul> <li> <p>UNCONFIRMED\
  \ - User has been created but not confirmed.</p> </li> <li> <p>CONFIRMED - User has been confirmed.</p> </li> <li> <p>UNKNOWN - User status isn't known.</p> </li> <li> <p>RESET_REQUIRED - User is confirmed, but the user must request a code and reset their password before they can sign in.</p> </li> <li> <p>FORCE_CHANGE_PASSWORD - The user is confirmed and the user can sign in using a temporary password, but on first sign-in, the user must change their password to a new value before doing anything else. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"MFAOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MFAOptionListType\"\n        },\n        {\n          \"description\": \" <i>This response parameter is no longer supported.</i> It provides information only about SMS MFA configurations. It doesn't provide information about time-based one-time password (TOTP) software token MFA configurations. To look up information about either type of MFA configuration,\
  \ use UserMFASettingList instead.\"\n        }\n      ]\n    },\n    \"PreferredMfaSetting\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The user's preferred MFA setting.\"\n        }\n      ]\n    },\n    \"UserMFASettingList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserMFASettingListType\"\n        },\n        {\n          \"description\": \"The MFA options that are activated for the user. The possible values in this list are <code>SMS_MFA</code> and <code>SOFTWARE_TOKEN_MFA</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Username\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-get-user-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: AdminGetUserResponse
---
