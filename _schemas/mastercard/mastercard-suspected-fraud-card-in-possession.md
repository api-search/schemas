---
description: Flag to indicate if the card holder was in possession of the card at the time the fraud occurred. Possible values are 'Y', 'N' and 'U' (for Unknown). This field is required for Issuer and optional for Acquirer. This is a conditional parameter and is mandatory when operationType value is CONFIRMED_FRAUD.
layout: schema
name: CardInPossession
properties_list: []
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-suspected-fraud-card-in-possession-schema.json
slug: mastercard-suspected-fraud-card-in-possession
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CardInPossession\",\n  \"type\": \"string\",\n  \"description\": \"Flag to indicate if the card holder was in possession of the card at the time the fraud occurred. Possible values are 'Y', 'N' and 'U' (for Unknown). This field is required for Issuer and optional for Acquirer. This is a conditional parameter and is mandatory when operationType value is CONFIRMED_FRAUD.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-suspected-fraud-card-in-possession-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: CardInPossession
---
