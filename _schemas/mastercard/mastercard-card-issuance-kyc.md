---
description: ''
layout: schema
name: Kyc
properties_list:
- description: KYC status of the client. If the status is true it indicates that KYC data has been updated and KYC completed. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </
  name: status
  type: boolean
- description: Remarks on the KYC status or documents. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required when KYC status is true.
  name: remark
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-kyc-schema.json
slug: mastercard-card-issuance-kyc
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Kyc\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"boolean\",\n      \"description\": \"KYC status of the client. If the status is true it indicates that KYC data has been updated and KYC completed. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"remark\": {\n      \"type\": \"string\",\n      \"description\": \"Remarks on the KYC status or documents. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required when KYC status is true.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-kyc-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Kyc
---
