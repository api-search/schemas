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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-ping-result-model-schema.json\",\n  \"title\": \"PingResultModel\",\n  \"description\": \"PingResultModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"AvaTax API version\"\n    },\n    \"authenticated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the request was authenticated\"\n    },\n    \"authenticationType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"None\",\n        \"UsernamePassword\",\n        \"AccountIdLicenseKey\",\n        \"OpenIdBearerToken\"\n      ],\n      \"description\": \"Type of authentication used\"\n    },\n    \"authenticatedUserName\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the authenticated user\"\n\
  \    },\n    \"authenticatedUserId\": {\n      \"type\": \"integer\",\n      \"description\": \"User ID of the authenticated user\"\n    },\n    \"authenticatedAccountId\": {\n      \"type\": \"integer\",\n      \"description\": \"Account ID of the authenticated user\"\n    },\n    \"crmid\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-ping-result-model-schema.json
tags:
- Taxes
title: PingResultModel
---
