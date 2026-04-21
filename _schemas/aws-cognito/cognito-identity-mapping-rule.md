---
description: A rule that maps a claim name, a claim value, and a match type to a role ARN.
layout: schema
name: MappingRule
properties_list:
- description: ''
  name: Claim
  type: object
- description: ''
  name: MatchType
  type: object
- description: ''
  name: Value
  type: object
- description: ''
  name: RoleARN
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-mapping-rule-schema.json
slug: cognito-identity-mapping-rule
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: MappingRule
---
