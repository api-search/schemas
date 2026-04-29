---
description: 'An indicator to help explain the status of the account being inquired on. Possible values are: * `VALID` = Matches the account as reported by the issuer. * `UNKNOWN` = Account number is not known to ABU or part of a participating BIN (Bank Identification Number) and/or issuer. * `NON_PARTICIPATING` = Account number is not known to ABU or part of a non-participating BIN (Bank Identification Number) and/or issuer. * `CONTACT` (C) = Contact the issuer. * `EXPIRY` (E) = The card inquired on is expired, updated expiry date returned. * `ACCOUNT_UPDATE` (A) = The card inquired on is updated, updated card number and expiry date returned.'
layout: schema
name: ResponseIndicator
properties_list: []
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-automatic-billing-updater-response-indicator-schema.json
slug: mastercard-automatic-billing-updater-response-indicator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseIndicator\",\n  \"type\": \"string\",\n  \"description\": \"An indicator to help explain the status of the account being inquired on. Possible values are:\\n* `VALID` = Matches the account as reported by the issuer.\\n* `UNKNOWN` = Account number is not known to ABU or part of a participating BIN (Bank Identification Number) and/or issuer.\\n* `NON_PARTICIPATING` = Account number is not known to ABU or part of a non-participating BIN (Bank Identification Number) and/or issuer.\\n* `CONTACT` (C) = Contact the issuer.\\n* `EXPIRY` (E) = The card inquired on is expired, updated expiry date returned.\\n* `ACCOUNT_UPDATE` (A) = The card inquired on is updated, updated card number and expiry date returned.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-automatic-billing-updater-response-indicator-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ResponseIndicator
---
