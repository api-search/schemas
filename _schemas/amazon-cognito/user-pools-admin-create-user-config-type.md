---
description: The configuration for creating a new user profile.
layout: schema
name: AdminCreateUserConfigType
properties_list:
- description: ''
  name: AllowAdminCreateUserOnly
  type: object
- description: ''
  name: UnusedAccountValidityDays
  type: object
- description: ''
  name: InviteMessageTemplate
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-admin-create-user-config-type-schema.json
slug: user-pools-admin-create-user-config-type
source_filename: user-pools-admin-create-user-config-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-create-user-config-type-schema.json\",\n  \"title\": \"AdminCreateUserConfigType\",\n  \"description\": \"The configuration for creating a new user profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AllowAdminCreateUserOnly\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"Set to <code>True</code> if only the administrator is allowed to create user profiles. Set to <code>False</code> if users can sign themselves up via an app.\"\n        }\n      ]\n    },\n    \"UnusedAccountValidityDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdminCreateUserUnusedAccountValidityDaysType\"\n        },\n        {\n          \"description\": \"<p>The user\
  \ account expiration limit, in days, after which a new account that hasn't signed in is no longer usable. To reset the account after that time limit, you must call <code>AdminCreateUser</code> again, specifying <code>\\\"RESEND\\\"</code> for the <code>MessageAction</code> parameter. The default value for this parameter is 7. </p> <note> <p>If you set a value for <code>TemporaryPasswordValidityDays</code> in <code>PasswordPolicy</code>, that value will be used, and <code>UnusedAccountValidityDays</code> will be no longer be an available parameter for that user pool.</p> </note>\"\n        }\n      ]\n    },\n    \"InviteMessageTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MessageTemplateType\"\n        },\n        {\n          \"description\": \"<p>The message template to be used for the welcome message to new users.</p> <p>See also <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pool-settings-message-customizations.html#cognito-user-pool-settings-user-invitation-message-customization\\\
  \">Customizing User Invitation Messages</a>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-create-user-config-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: AdminCreateUserConfigType
---
