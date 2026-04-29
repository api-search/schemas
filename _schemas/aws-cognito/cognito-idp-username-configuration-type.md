---
description: The username configuration type.
layout: schema
name: UsernameConfigurationType
properties_list:
- description: ''
  name: CaseSensitive
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-username-configuration-type-schema.json
slug: cognito-idp-username-configuration-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"CaseSensitive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrappedBooleanType\"\n        },\n        {\n          \"description\": \"<p>Specifies whether user name case sensitivity will be applied for all users in the user pool through Amazon Cognito APIs.</p> <p>Valid values include:</p> <dl> <dt>True</dt> <dd> <p>Enables case sensitivity for all username input. When this option is set to <code>True</code>, users must sign in using the exact capitalization of their given username, such as \\u201cUserName\\u201d. This is the default value.</p> </dd> <dt>False</dt> <dd> <p>Enables case insensitivity for all username input. For example, when this option is set to <code>False</code>, users can sign in using either \\\"username\\\" or \\\"Username\\\". This option also enables both <code>preferred_username</code> and <code>email</code> alias to be case insensitive, in addition to the <code>username</code>\
  \ attribute.</p> </dd> </dl>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CaseSensitive\"\n  ],\n  \"description\": \"The username configuration type. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-username-configuration-type-schema.json\",\n  \"title\": \"UsernameConfigurationType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-username-configuration-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UsernameConfigurationType
---
