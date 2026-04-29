---
description: BillingAccount schema from Ampersand API
layout: schema
name: BillingAccount
properties_list:
- description: The billing account ID.
  name: id
  type: string
- description: The display name of the billing account.
  name: displayName
  type: string
- description: The billing provider that this account is associated with.
  name: billingProvider
  type: string
- description: The ID used by the billing provider to identify the account.
  name: billingProviderRef
  type: string
- description: The time the billing account was created.
  name: createTime
  type: string
- description: The time the billing account was last updated.
  name: updateTime
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-billing-account-schema.json
slug: ampersand-api-billing-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-billing-account-schema.json\",\n  \"title\": \"BillingAccount\",\n  \"description\": \"BillingAccount schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The billing account ID.\",\n      \"example\": \"billing-account-123\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the billing account.\",\n      \"example\": \"Acme Inc\"\n    },\n    \"billingProvider\": {\n      \"type\": \"string\",\n      \"description\": \"The billing provider that this account is associated with.\",\n      \"example\": \"stripe\"\n    },\n    \"billingProviderRef\": {\n      \"type\": \"string\",\n      \"description\": \"The ID used by the billing provider to identify\
  \ the account.\",\n      \"example\": \"acct_1J2k3l4m5n6o7p8q9r0s\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the billing account was created.\",\n      \"format\": \"date-time\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the billing account was last updated.\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"displayName\",\n    \"billingProvider\",\n    \"billingProviderRef\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-billing-account-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: BillingAccount
---
