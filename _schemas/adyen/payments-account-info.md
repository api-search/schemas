---
description: AccountInfo schema from Adyen API
layout: schema
name: AccountInfo
properties_list:
- description: 'Indicator for the length of time since this shopper account was created in the merchant''s environment. Allowed values: * notApplicable * thisTransaction * lessThan30Days * from30To60Days * moreThan60D'
  name: accountAgeIndicator
  type: string
- description: Date when the shopper's account was last changed.
  name: accountChangeDate
  type: string
- description: 'Indicator for the length of time since the shopper''s account was last updated. Allowed values: * thisTransaction * lessThan30Days * from30To60Days * moreThan60Days'
  name: accountChangeIndicator
  type: string
- description: Date when the shopper's account was created.
  name: accountCreationDate
  type: string
- description: 'Indicates the type of account. For example, for a multi-account card product. Allowed values: * notApplicable * credit * debit'
  name: accountType
  type: string
- description: Number of attempts the shopper tried to add a card to their account in the last day.
  name: addCardAttemptsDay
  type: integer
- description: Date the selected delivery address was first used.
  name: deliveryAddressUsageDate
  type: string
- description: 'Indicator for the length of time since this delivery address was first used. Allowed values: * thisTransaction * lessThan30Days * from30To60Days * moreThan60Days'
  name: deliveryAddressUsageIndicator
  type: string
- description: Shopper's home phone number (including the country code).
  name: homePhone
  type: string
- description: Shopper's mobile phone number (including the country code).
  name: mobilePhone
  type: string
- description: Date when the shopper last changed their password.
  name: passwordChangeDate
  type: string
- description: 'Indicator when the shopper has changed their password. Allowed values: * notApplicable * thisTransaction * lessThan30Days * from30To60Days * moreThan60Days'
  name: passwordChangeIndicator
  type: string
- description: Number of all transactions (successful and abandoned) from this shopper in the past 24 hours.
  name: pastTransactionsDay
  type: integer
- description: Number of all transactions (successful and abandoned) from this shopper in the past year.
  name: pastTransactionsYear
  type: integer
- description: Date this payment method was added to the shopper's account.
  name: paymentAccountAge
  type: string
- description: 'Indicator for the length of time since this payment method was added to this shopper''s account. Allowed values: * notApplicable * thisTransaction * lessThan30Days * from30To60Days * moreThan60Days'
  name: paymentAccountIndicator
  type: string
- description: Number of successful purchases in the last six months.
  name: purchasesLast6Months
  type: integer
- description: Whether suspicious activity was recorded on this account.
  name: suspiciousActivity
  type: boolean
- description: Shopper's work phone number (including the country code).
  name: workPhone
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-account-info-schema.json
slug: payments-account-info
source_filename: payments-account-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-account-info-schema.json\",\n  \"title\": \"AccountInfo\",\n  \"description\": \"AccountInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountAgeIndicator\": {\n      \"description\": \"Indicator for the length of time since this shopper account was created in the merchant's environment.\\nAllowed values:\\n* notApplicable\\n* thisTransaction\\n* lessThan30Days\\n* from30To60Days\\n* moreThan60Days\",\n      \"enum\": [\n        \"notApplicable\",\n        \"thisTransaction\",\n        \"lessThan30Days\",\n        \"from30To60Days\",\n        \"moreThan60Days\"\n      ],\n      \"type\": \"string\"\n    },\n    \"accountChangeDate\": {\n      \"description\": \"Date when the shopper's account was last changed.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\
  \n    },\n    \"accountChangeIndicator\": {\n      \"description\": \"Indicator for the length of time since the shopper's account was last updated.\\nAllowed values:\\n* thisTransaction\\n* lessThan30Days\\n* from30To60Days\\n* moreThan60Days\",\n      \"enum\": [\n        \"thisTransaction\",\n        \"lessThan30Days\",\n        \"from30To60Days\",\n        \"moreThan60Days\"\n      ],\n      \"type\": \"string\"\n    },\n    \"accountCreationDate\": {\n      \"description\": \"Date when the shopper's account was created.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"accountType\": {\n      \"x-addedInVersion\": \"50\",\n      \"description\": \"Indicates the type of account. For example, for a multi-account card product.\\nAllowed values:\\n* notApplicable\\n* credit\\n* debit\",\n      \"enum\": [\n        \"notApplicable\",\n        \"credit\",\n        \"debit\"\n      ],\n      \"type\": \"string\"\n    },\n    \"addCardAttemptsDay\": {\n     \
  \ \"description\": \"Number of attempts the shopper tried to add a card to their account in the last day.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"deliveryAddressUsageDate\": {\n      \"description\": \"Date the selected delivery address was first used.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"deliveryAddressUsageIndicator\": {\n      \"description\": \"Indicator for the length of time since this delivery address was first used.\\nAllowed values:\\n* thisTransaction\\n* lessThan30Days\\n* from30To60Days\\n* moreThan60Days\",\n      \"enum\": [\n        \"thisTransaction\",\n        \"lessThan30Days\",\n        \"from30To60Days\",\n        \"moreThan60Days\"\n      ],\n      \"type\": \"string\"\n    },\n    \"homePhone\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"68\",\n      \"x-deprecatedMessage\": \"Use `ThreeDS2RequestData.homePhone` instead.\",\n      \"description\": \"Shopper's home\
  \ phone number (including the country code).\",\n      \"type\": \"string\"\n    },\n    \"mobilePhone\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"68\",\n      \"x-deprecatedMessage\": \"Use `ThreeDS2RequestData.mobilePhone` instead.\",\n      \"description\": \"Shopper's mobile phone number (including the country code).\",\n      \"type\": \"string\"\n    },\n    \"passwordChangeDate\": {\n      \"description\": \"Date when the shopper last changed their password.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"passwordChangeIndicator\": {\n      \"description\": \"Indicator when the shopper has changed their password.\\nAllowed values:\\n* notApplicable\\n* thisTransaction\\n* lessThan30Days\\n* from30To60Days\\n* moreThan60Days\",\n      \"enum\": [\n        \"notApplicable\",\n        \"thisTransaction\",\n        \"lessThan30Days\",\n        \"from30To60Days\",\n        \"moreThan60Days\"\n      ],\n      \"type\": \"string\"\
  \n    },\n    \"pastTransactionsDay\": {\n      \"description\": \"Number of all transactions (successful and abandoned) from this shopper in the past 24 hours.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"pastTransactionsYear\": {\n      \"description\": \"Number of all transactions (successful and abandoned) from this shopper in the past year.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"paymentAccountAge\": {\n      \"description\": \"Date this payment method was added to the shopper's account.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"paymentAccountIndicator\": {\n      \"description\": \"Indicator for the length of time since this payment method was added to this shopper's account.\\nAllowed values:\\n* notApplicable\\n* thisTransaction\\n* lessThan30Days\\n* from30To60Days\\n* moreThan60Days\",\n      \"enum\": [\n        \"notApplicable\",\n        \"thisTransaction\",\n       \
  \ \"lessThan30Days\",\n        \"from30To60Days\",\n        \"moreThan60Days\"\n      ],\n      \"type\": \"string\"\n    },\n    \"purchasesLast6Months\": {\n      \"description\": \"Number of successful purchases in the last six months.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"suspiciousActivity\": {\n      \"description\": \"Whether suspicious activity was recorded on this account.\",\n      \"type\": \"boolean\"\n    },\n    \"workPhone\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"68\",\n      \"x-deprecatedMessage\": \"Use `ThreeDS2RequestData.workPhone` instead.\",\n      \"description\": \"Shopper's work phone number (including the country code).\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-account-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountInfo
---
