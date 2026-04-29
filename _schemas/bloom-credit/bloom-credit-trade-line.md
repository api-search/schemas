---
description: An individual account or trade line in a credit report.
layout: schema
name: TradeLine
properties_list:
- description: Unique identifier for this trade line.
  name: account_id
  type: string
- description: Bureau reporting this trade line.
  name: bureau
  type: string
- description: Name of the creditor or lender.
  name: creditor_name
  type: string
- description: Type of account.
  name: account_type
  type: string
- description: Whether the account is open or closed.
  name: account_status
  type: string
- description: Credit limit in USD.
  name: credit_limit
  type: integer
- description: Current balance in USD.
  name: current_balance
  type: integer
- description: Current payment status.
  name: payment_status
  type: string
- description: ''
  name: opened_date
  type: string
- description: ''
  name: last_activity_date
  type: string
provider_name: Bloom Credit
provider_slug: bloom-credit
schema_file: json-schema/bloom-credit-trade-line-schema.json
slug: bloom-credit-trade-line
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bloom-credit/main/json-schema/bloom-credit-trade-line-schema.json\",\n  \"title\": \"TradeLine\",\n  \"description\": \"An individual account or trade line in a credit report.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this trade line.\",\n      \"example\": \"tl_9a8b7c6d5e4f\"\n    },\n    \"bureau\": {\n      \"type\": \"string\",\n      \"description\": \"Bureau reporting this trade line.\",\n      \"enum\": [\"equifax\", \"experian\", \"transunion\"],\n      \"example\": \"equifax\"\n    },\n    \"creditor_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the creditor or lender.\",\n      \"example\": \"Chase Bank\"\n    },\n    \"account_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of account.\"\
  ,\n      \"example\": \"revolving\"\n    },\n    \"account_status\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the account is open or closed.\",\n      \"enum\": [\"open\", \"closed\"],\n      \"example\": \"open\"\n    },\n    \"credit_limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Credit limit in USD.\",\n      \"example\": 10000\n    },\n    \"current_balance\": {\n      \"type\": \"integer\",\n      \"description\": \"Current balance in USD.\",\n      \"example\": 2400\n    },\n    \"payment_status\": {\n      \"type\": \"string\",\n      \"description\": \"Current payment status.\",\n      \"example\": \"current\"\n    },\n    \"opened_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2018-03-01\"\n    },\n    \"last_activity_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2026-01-10\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloom-credit/refs/heads/main/json-schema/bloom-credit-trade-line-schema.json
tags:
- Credit Bureau
- Credit Reports
- Credit Scores
- Fintech
- Lending
- Personal Finance
title: TradeLine
---
