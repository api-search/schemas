---
description: Account takeover action type.
layout: schema
name: AccountTakeoverActionType
properties_list:
- description: ''
  name: Notify
  type: object
- description: ''
  name: EventAction
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-account-takeover-action-type-schema.json
slug: cognito-idp-account-takeover-action-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Notify\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountTakeoverActionNotifyType\"\n        },\n        {\n          \"description\": \"Flag specifying whether to send a notification.\"\n        }\n      ]\n    },\n    \"EventAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountTakeoverEventActionType\"\n        },\n        {\n          \"description\": \"<p>The action to take in response to the account takeover action. Valid values are as follows:</p> <ul> <li> <p> <code>BLOCK</code> Choosing this action will block the request.</p> </li> <li> <p> <code>MFA_IF_CONFIGURED</code> Present an MFA challenge if user has configured it, else allow the request.</p> </li> <li> <p> <code>MFA_REQUIRED</code> Present an MFA challenge if user has configured it, else block the request.</p> </li> <li> <p> <code>NO_ACTION</code> Allow the user to sign in.</p>\
  \ </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Notify\",\n    \"EventAction\"\n  ],\n  \"description\": \"Account takeover action type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-account-takeover-action-type-schema.json\",\n  \"title\": \"AccountTakeoverActionType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-account-takeover-action-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AccountTakeoverActionType
---
