---
description: ''
layout: schema
name: Application
properties_list:
- description: Client on-boarding application form number.
  name: formNumber
  type: string
- description: 'Indicates whether the application should go through the checker approval process prior to client on-boarding. Applicable only if not requested for ''instant card''. It will be always considered as true '
  name: makerChecker
  type: boolean
- description: Free text field that contains remarks entered while submitting the request. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: memo
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-application-schema.json
slug: mastercard-card-issuance-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Application\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"formNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Client on-boarding application form number.\"\n    },\n    \"makerChecker\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the application should go through the checker approval process prior to client on-boarding. Applicable only if not requested for 'instant card'. It will be always considered as true in case of 'instant card' or 'SVC/LVC' card issuance irrespective of input value.\"\n    },\n    \"memo\": {\n      \"type\": \"string\",\n      \"description\": \"Free text field that contains remarks entered while submitting the request. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-application-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Application
---
