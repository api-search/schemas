---
description: The request representing the confirmation for a password reset.
layout: schema
name: ConfirmForgotPasswordRequest
properties_list:
- description: ''
  name: ClientId
  type: object
- description: ''
  name: SecretHash
  type: object
- description: ''
  name: Username
  type: object
- description: ''
  name: ConfirmationCode
  type: object
- description: ''
  name: Password
  type: object
- description: ''
  name: AnalyticsMetadata
  type: object
- description: ''
  name: UserContextData
  type: object
- description: ''
  name: ClientMetadata
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-confirm-forgot-password-request-schema.json
slug: cognito-idp-confirm-forgot-password-request
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ConfirmForgotPasswordRequest
---
