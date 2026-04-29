---
description: SetupBeneficiaryRequest schema from Adyen API
layout: schema
name: SetupBeneficiaryRequest
properties_list:
- description: The destination account code.
  name: destinationAccountCode
  type: string
- description: A value that can be supplied at the discretion of the executing user.
  name: merchantReference
  type: string
- description: The benefactor account.
  name: sourceAccountCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-setup-beneficiary-request-schema.json
slug: funds-setup-beneficiary-request
source_filename: funds-setup-beneficiary-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-setup-beneficiary-request-schema.json\",\n  \"title\": \"SetupBeneficiaryRequest\",\n  \"description\": \"SetupBeneficiaryRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destinationAccountCode\": {\n      \"description\": \"The destination account code.\",\n      \"type\": \"string\"\n    },\n    \"merchantReference\": {\n      \"description\": \"A value that can be supplied at the discretion of the executing user.\",\n      \"type\": \"string\"\n    },\n    \"sourceAccountCode\": {\n      \"description\": \"The benefactor account.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"sourceAccountCode\",\n    \"destinationAccountCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-setup-beneficiary-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SetupBeneficiaryRequest
---
