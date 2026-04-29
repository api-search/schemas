---
description: The type of the configuration to override the risk decision.
layout: schema
name: RiskExceptionConfigurationType
properties_list:
- description: ''
  name: BlockedIPRangeList
  type: object
- description: ''
  name: SkippedIPRangeList
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-risk-exception-configuration-type-schema.json
slug: cognito-idp-risk-exception-configuration-type
source_filename: cognito-idp-risk-exception-configuration-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlockedIPRangeList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockedIPRangeListType\"\n        },\n        {\n          \"description\": \"Overrides the risk decision to always block the pre-authentication requests. The IP range is in CIDR notation, a compact representation of an IP address and its routing prefix.\"\n        }\n      ]\n    },\n    \"SkippedIPRangeList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SkippedIPRangeListType\"\n        },\n        {\n          \"description\": \"Risk detection isn't performed on the IP addresses in this range list. The IP range is in CIDR notation.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The type of the configuration to override the risk decision.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-risk-exception-configuration-type-schema.json\"\
  ,\n  \"title\": \"RiskExceptionConfigurationType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-risk-exception-configuration-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: RiskExceptionConfigurationType
---
