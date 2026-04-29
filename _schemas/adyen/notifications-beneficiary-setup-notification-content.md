---
description: BeneficiarySetupNotificationContent schema from Adyen API
layout: schema
name: BeneficiarySetupNotificationContent
properties_list:
- description: The code of the beneficiary account.
  name: destinationAccountCode
  type: string
- description: The code of the beneficiary Account Holder.
  name: destinationAccountHolderCode
  type: string
- description: A listing of the invalid fields which have caused the Setup Beneficiary request to fail. If this is empty, the Setup Beneficiary request has succeeded.
  name: invalidFields
  type: array
- description: The reference provided by the merchant.
  name: merchantReference
  type: string
- description: The code of the benefactor account.
  name: sourceAccountCode
  type: string
- description: The code of the benefactor Account Holder.
  name: sourceAccountHolderCode
  type: string
- description: The date on which the beneficiary was set up and funds transferred from benefactor to beneficiary.
  name: transferDate
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-beneficiary-setup-notification-content-schema.json
slug: notifications-beneficiary-setup-notification-content
source_filename: notifications-beneficiary-setup-notification-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-beneficiary-setup-notification-content-schema.json\",\n  \"title\": \"BeneficiarySetupNotificationContent\",\n  \"description\": \"BeneficiarySetupNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destinationAccountCode\": {\n      \"description\": \"The code of the beneficiary account.\",\n      \"type\": \"string\"\n    },\n    \"destinationAccountHolderCode\": {\n      \"description\": \"The code of the beneficiary Account Holder.\",\n      \"type\": \"string\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"A listing of the invalid fields which have caused the Setup Beneficiary request to fail. If this is empty, the Setup Beneficiary request has succeeded.\",\n      \"items\": {\n        \"$ref\": \"\
  #/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantReference\": {\n      \"description\": \"The reference provided by the merchant.\",\n      \"type\": \"string\"\n    },\n    \"sourceAccountCode\": {\n      \"description\": \"The code of the benefactor account.\",\n      \"type\": \"string\"\n    },\n    \"sourceAccountHolderCode\": {\n      \"description\": \"The code of the benefactor Account Holder.\",\n      \"type\": \"string\"\n    },\n    \"transferDate\": {\n      \"description\": \"The date on which the beneficiary was set up and funds transferred from benefactor to beneficiary.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-beneficiary-setup-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BeneficiarySetupNotificationContent
---
