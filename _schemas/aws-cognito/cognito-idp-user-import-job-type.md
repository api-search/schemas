---
description: The user import job type.
layout: schema
name: UserImportJobType
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: JobId
  type: object
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: PreSignedUrl
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: StartDate
  type: object
- description: ''
  name: CompletionDate
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CloudWatchLogsRoleArn
  type: object
- description: ''
  name: ImportedUsers
  type: object
- description: ''
  name: SkippedUsers
  type: object
- description: ''
  name: FailedUsers
  type: object
- description: ''
  name: CompletionMessage
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-user-import-job-type-schema.json
slug: cognito-idp-user-import-job-type
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UserImportJobType
---
