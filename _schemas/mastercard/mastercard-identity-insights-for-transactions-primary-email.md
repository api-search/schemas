---
description: ''
layout: schema
name: PrimaryEmail
properties_list:
- description: Count of days since the email was first observed in Ekata's Identity Network. If the email has not been observed before, first_seen_days will be 0.
  name: firstSeenDays
  type: integer
- description: Number of days that have passed since the email address was last seen.
  name: lastSeenDays
  type: integer
- description: True if the email address is valid
  name: valid
  type: boolean
- description: The date when the email domain was created. Format is YYYY-MM-DD.
  name: domainCreationDate
  type: string
- description: The match status between the input name and the queried entity.
  name: matchToName
  type: string
- description: Number of times email has been seen in last 180 days.
  name: mailboxVelocity
  type: integer
- description: True if the email domain is disposable. Disposable emails are generally associated with fraudulent activities. If true, this is one of the strongest risk indicators and the transaction should be flagg
  name: isDisposable
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-primary-email-schema.json
slug: mastercard-identity-insights-for-transactions-primary-email
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PrimaryEmail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstSeenDays\": {\n      \"type\": \"integer\",\n      \"description\": \"Count of days since the email was first observed in Ekata's Identity Network. If the email has not been observed before, first_seen_days will be 0.\"\n    },\n    \"lastSeenDays\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of days that have passed since the email address was last seen.\"\n    },\n    \"valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the email address is valid\"\n    },\n    \"domainCreationDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date when the email domain was created. Format is YYYY-MM-DD.\"\n    },\n    \"matchToName\": {\n      \"type\": \"string\",\n      \"description\": \"The match status between the input name and the queried entity.\"\n    },\n    \"\
  mailboxVelocity\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times email has been seen in last 180 days.\"\n    },\n    \"isDisposable\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the email domain is disposable. Disposable emails are generally associated with fraudulent activities. If true, this is one of the strongest risk indicators and the transaction should be flagged for further review.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-primary-email-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: PrimaryEmail
---
