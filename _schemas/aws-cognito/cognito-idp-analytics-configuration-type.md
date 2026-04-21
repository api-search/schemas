---
description: <p>The Amazon Pinpoint analytics configuration necessary to collect metrics for a user pool.</p> <note> <p>In Regions where Amazon Pinpointisn't available, user pools only support sending events to Amazon Pinpoint projects in us-east-1. In Regions where Amazon Pinpoint is available, user pools support sending events to Amazon Pinpoint projects within that same Region.</p> </note>
layout: schema
name: AnalyticsConfigurationType
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: ApplicationArn
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: ExternalId
  type: object
- description: ''
  name: UserDataShared
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-analytics-configuration-type-schema.json
slug: cognito-idp-analytics-configuration-type
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AnalyticsConfigurationType
---
