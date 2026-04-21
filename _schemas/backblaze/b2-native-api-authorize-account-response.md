---
description: Response from the b2_authorize_account operation
layout: schema
name: AuthorizeAccountResponse
properties_list:
- description: The identifier for the account
  name: accountId
  type: string
- description: An authorization token to use with all calls other than b2_authorize_account
  name: authorizationToken
  type: string
- description: ''
  name: allowed
  type: object
- description: ''
  name: apiInfo
  type: object
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-authorize-account-response-schema.json
slug: b2-native-api-authorize-account-response
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: AuthorizeAccountResponse
---
