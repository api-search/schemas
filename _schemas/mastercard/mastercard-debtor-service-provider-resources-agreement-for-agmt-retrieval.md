---
description: ''
layout: schema
name: AgreementForAgmtRetrieval
properties_list:
- description: Unique identifier assigned by Mastercard to the agreement.
  name: agreementId
  type: string
- description: Unique 6 digit reference used by DSP to retrieve the create agreement request.
  name: agreementReferenceNumber
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-agreement-for-agmt-retrieval-schema.json
slug: mastercard-debtor-service-provider-resources-agreement-for-agmt-retrieval
source_filename: mastercard-debtor-service-provider-resources-agreement-for-agmt-retrieval-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgreementForAgmtRetrieval\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agreementId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned by Mastercard to the agreement.\"\n    },\n    \"agreementReferenceNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Unique 6 digit reference used by DSP to retrieve the create agreement request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-agreement-for-agmt-retrieval-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AgreementForAgmtRetrieval
---
