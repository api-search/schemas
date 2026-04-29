---
description: ''
layout: schema
name: AgreementForAgmtUpdate
properties_list:
- description: Unique identifier assigned by Mastercard to the agreement.
  name: agreementId
  type: string
- description: Status of the Agreement updated by DSP to either Approved or Rejected or Deleted. * Refer to Codes and Formats section for more details.
  name: agreementStatus
  type: string
- description: Reason provided by DSP when agreement status is rejected. * Refer to Codes and Formats section for more details.
  name: agreementStatusReason
  type: string
- description: Nickname updated by DSP. Nickname must be supplied when agreement status is Approved.
  name: accountNickname
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-agreement-for-agmt-update-schema.json
slug: mastercard-debtor-service-provider-resources-agreement-for-agmt-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgreementForAgmtUpdate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agreementId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned by Mastercard to the agreement.\"\n    },\n    \"agreementStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the Agreement updated by DSP to either Approved or Rejected or Deleted. * Refer to Codes and Formats section for more details.\"\n    },\n    \"agreementStatusReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason provided by DSP when agreement status is rejected. * Refer to Codes and Formats section for more details.\"\n    },\n    \"accountNickname\": {\n      \"type\": \"string\",\n      \"description\": \"Nickname updated by DSP. Nickname must be supplied when agreement status is Approved.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-agreement-for-agmt-update-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AgreementForAgmtUpdate
---
