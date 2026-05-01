---
description: <p>User pool add-ons. Contains settings for activation of advanced security features. To log user security information but take no action, set to <code>AUDIT</code>. To configure automatic security responses to risky traffic to your user pool, set to <code>ENFORCED</code>.</p> <p>For more information, see <a href="https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pool-settings-advanced-security.html">Adding advanced security to a user pool</a>.</p>
layout: schema
name: UserPoolAddOnsType
properties_list:
- description: ''
  name: AdvancedSecurityMode
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-user-pool-add-ons-type-schema.json
slug: user-pools-user-pool-add-ons-type
source_filename: user-pools-user-pool-add-ons-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-pool-add-ons-type-schema.json\",\n  \"title\": \"UserPoolAddOnsType\",\n  \"description\": \"<p>User pool add-ons. Contains settings for activation of advanced security features. To log user security information but take no action, set to <code>AUDIT</code>. To configure automatic security responses to risky traffic to your user pool, set to <code>ENFORCED</code>.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pool-settings-advanced-security.html\\\">Adding advanced security to a user pool</a>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdvancedSecurityMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdvancedSecurityModeType\"\n        },\n        {\n          \"description\"\
  : \"The operating mode of advanced security features in your user pool.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AdvancedSecurityMode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-pool-add-ons-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: UserPoolAddOnsType
---
