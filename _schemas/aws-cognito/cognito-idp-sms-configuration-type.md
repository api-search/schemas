---
description: The SMS configuration type is the settings that your Amazon Cognito user pool must use to send an SMS message from your Amazon Web Services account through Amazon Simple Notification Service. To send SMS messages with Amazon SNS in the Amazon Web Services Region that you want, the Amazon Cognito user pool uses an Identity and Access Management (IAM) role in your Amazon Web Services account.
layout: schema
name: SmsConfigurationType
properties_list:
- description: ''
  name: SnsCallerArn
  type: object
- description: ''
  name: ExternalId
  type: object
- description: ''
  name: SnsRegion
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-sms-configuration-type-schema.json
slug: cognito-idp-sms-configuration-type
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: SmsConfigurationType
---
