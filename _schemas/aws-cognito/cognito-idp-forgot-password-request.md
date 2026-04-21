---
description: Represents the request to reset a user's password.
layout: schema
name: ForgotPasswordRequest
properties_list:
- description: ''
  name: ClientId
  type: object
- description: ''
  name: SecretHash
  type: object
- description: ''
  name: UserContextData
  type: object
- description: ''
  name: Username
  type: object
- description: ''
  name: AnalyticsMetadata
  type: object
- description: ''
  name: ClientMetadata
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-forgot-password-request-schema.json
slug: cognito-idp-forgot-password-request
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ForgotPasswordRequest
---
