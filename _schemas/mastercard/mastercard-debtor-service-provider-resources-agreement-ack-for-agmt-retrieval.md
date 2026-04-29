---
description: ''
layout: schema
name: AgreementAckForAgmtRetrieval
properties_list:
- description: Unique identifier assigned by Mastercard to the agreement.
  name: agreementId
  type: string
- description: Creditor requesting DSP to display to Debtor to setup Agreement during payment confirmation. * Refer to Codes and Formats section for more details.
  name: agreementType
  type: string
- description: Status of the Agreement. * Refer to Codes and Formats section for more details.
  name: agreementStatus
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-agreement-ack-for-agmt-retrieval-schema.json
slug: mastercard-debtor-service-provider-resources-agreement-ack-for-agmt-retrieval
source_filename: mastercard-debtor-service-provider-resources-agreement-ack-for-agmt-retrieval-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgreementAckForAgmtRetrieval\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agreementId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned by Mastercard to the agreement.\"\n    },\n    \"agreementType\": {\n      \"type\": \"string\",\n      \"description\": \"Creditor requesting DSP to display to Debtor to setup Agreement during payment confirmation. * Refer to Codes and Formats section for more details.\"\n    },\n    \"agreementStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the Agreement. * Refer to Codes and Formats section for more details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-agreement-ack-for-agmt-retrieval-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AgreementAckForAgmtRetrieval
---
