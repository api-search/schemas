---
description: 'Statement delivery options. <BR/> **Conditional Mandatory**<font color=''red''>* </font> field - Required while creating new client. <br/> Valid values are configured on ''Card Management > Institution Parameter Setup > System Codes [ISSS15]'' screen for ''Type Id=STATEMENT_PREFERENCE''. <br/> **Few sample values: ** * `Email` - Statement delivery via email * `Hard Copy` - Statement delivery via hard copy * `Both` - Statement delivery via email as well as hard copy'
layout: schema
name: StatementDeliveryOption
properties_list: []
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-statement-delivery-option-schema.json
slug: mastercard-card-issuance-statement-delivery-option
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatementDeliveryOption\",\n  \"type\": \"string\",\n  \"description\": \"Statement delivery options. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required while creating new client. <br/> Valid values are configured on 'Card Management > Institution Parameter Setup > System Codes [ISSS15]'     screen for 'Type Id=STATEMENT_PREFERENCE'. <br/> **Few sample values: **\\n* `Email` - Statement delivery via email\\n* `Hard Copy` - Statement delivery via hard copy\\n* `Both` - Statement delivery via email as well as hard copy\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-statement-delivery-option-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: StatementDeliveryOption
---
