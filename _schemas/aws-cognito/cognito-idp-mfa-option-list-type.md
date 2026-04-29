---
description: MFAOptionListType schema from Amazon Cognito
layout: schema
name: MFAOptionListType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-mfa-option-list-type-schema.json
slug: cognito-idp-mfa-option-list-type
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"DeliveryMedium\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DeliveryMediumType\"\n          },\n          {\n            \"description\": \"The delivery medium to send the MFA code. You can use this parameter to set only the <code>SMS</code> delivery medium value.\"\n          }\n        ]\n      },\n      \"AttributeName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AttributeNameType\"\n          },\n          {\n            \"description\": \"The attribute name of the MFA option type. The only valid value is <code>phone_number</code>.\"\n          }\n        ]\n      }\n    },\n    \"description\": \" <i>This data type is no longer supported.</i> Applies only to SMS multi-factor authentication (MFA) configurations. Does not apply to time-based one-time password (TOTP) software token MFA configurations.\"\
  \n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-mfa-option-list-type-schema.json\",\n  \"title\": \"MFAOptionListType\",\n  \"description\": \"MFAOptionListType schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-mfa-option-list-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: MFAOptionListType
---
