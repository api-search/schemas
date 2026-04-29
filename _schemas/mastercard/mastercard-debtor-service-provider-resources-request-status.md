---
description: ''
layout: schema
name: RequestStatus
properties_list:
- description: Status of the Payment Request returned by Mastercard. * Refer to Codes and Formats section for more details.
  name: paymentRequestStatus
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-request-status-schema.json
slug: mastercard-debtor-service-provider-resources-request-status
source_filename: mastercard-debtor-service-provider-resources-request-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequestStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paymentRequestStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the Payment Request returned by Mastercard. * Refer to Codes and Formats section for more details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-request-status-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: RequestStatus
---
