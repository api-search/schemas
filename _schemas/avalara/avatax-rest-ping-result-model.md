---
description: PingResultModel schema from Avalara API
layout: schema
name: PingResultModel
properties_list:
- description: AvaTax API version
  name: version
  type: string
- description: Whether the request was authenticated
  name: authenticated
  type: boolean
- description: Type of authentication used
  name: authenticationType
  type: string
- description: Username of the authenticated user
  name: authenticatedUserName
  type: string
- description: User ID of the authenticated user
  name: authenticatedUserId
  type: integer
- description: Account ID of the authenticated user
  name: authenticatedAccountId
  type: integer
- description: ''
  name: crmid
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-ping-result-model-schema.json
slug: avatax-rest-ping-result-model
tags:
- Taxes
title: PingResultModel
---
