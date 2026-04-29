---
description: The username configuration type.
layout: schema
name: UsernameConfigurationType
properties_list:
- description: ''
  name: CaseSensitive
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-username-configuration-type-schema.json
slug: user-pools-username-configuration-type
source_filename: user-pools-username-configuration-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-username-configuration-type-schema.json\",\n  \"title\": \"UsernameConfigurationType\",\n  \"description\": \"The username configuration type. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CaseSensitive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrappedBooleanType\"\n        },\n        {\n          \"description\": \"<p>Specifies whether user name case sensitivity will be applied for all users in the user pool through Amazon Cognito APIs. For most use cases, set case sensitivity to <code>False</code> (case insensitive) as a best practice. When usernames and email addresses are case insensitive, users can sign in as the same user when they enter a different capitalization of their user name.</p> <p>Valid values include:</p> <dl> <dt>True</dt> <dd>\
  \ <p>Enables case sensitivity for all username input. When this option is set to <code>True</code>, users must sign in using the exact capitalization of their given username, such as \\u201cUserName\\u201d. This is the default value.</p> </dd> <dt>False</dt> <dd> <p>Enables case insensitivity for all username input. For example, when this option is set to <code>False</code>, users can sign in using <code>username</code>, <code>USERNAME</code>, or <code>UserName</code>. This option also enables both <code>preferred_username</code> and <code>email</code> alias to be case insensitive, in addition to the <code>username</code> attribute.</p> </dd> </dl>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CaseSensitive\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-username-configuration-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UsernameConfigurationType
---
