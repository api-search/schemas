---
description: ''
layout: schema
name: AgreementForAgmtUpdate
properties_list:
- description: Unique identifier assigned by Mastercard to the agreement.
  name: agreementId
  type: string
- description: Status of the Agreement updated by CSP. * Refer to Codes and Formats section for more details.
  name: agreementStatus
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-agreement-for-agmt-update-schema.json
slug: mastercard-account-to-account-commerce-for-creditor-service-providers-agreement-for-agmt-update
source_filename: mastercard-account-to-account-commerce-for-creditor-service-providers-agreement-for-agmt-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgreementForAgmtUpdate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agreementId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned by Mastercard to the agreement.\"\n    },\n    \"agreementStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the Agreement updated by CSP. * Refer to Codes and Formats section for more details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-agreement-for-agmt-update-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AgreementForAgmtUpdate
---
