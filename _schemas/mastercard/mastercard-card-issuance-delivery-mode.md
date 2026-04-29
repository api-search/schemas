---
description: Client's preferred delivery mode. Application request with instant card true, delivery mode should be `Branch`. <br/> Valid values are configured on "Card Management > Institution Parameter Setup > System Codes [ISSS15]" screen for "Type Id=DELIVERY_MODE". <br/> **Few sample values:** `Branch`, `Payment system department`, `Mail`
layout: schema
name: DeliveryMode
properties_list: []
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-delivery-mode-schema.json
slug: mastercard-card-issuance-delivery-mode
source_filename: mastercard-card-issuance-delivery-mode-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeliveryMode\",\n  \"type\": \"string\",\n  \"description\": \"Client's preferred delivery mode. Application request with instant card true, delivery mode should be `Branch`. <br/> Valid values are configured on \\\"Card Management > Institution Parameter Setup > System Codes [ISSS15]\\\" screen for \\\"Type Id=DELIVERY_MODE\\\". <br/> **Few sample values:** `Branch`, `Payment system department`, `Mail`\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-delivery-mode-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: DeliveryMode
---
