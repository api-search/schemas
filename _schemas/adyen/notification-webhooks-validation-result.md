---
description: ValidationResult schema from Adyen API
layout: schema
name: ValidationResult
properties_list:
- description: 'The result of the check. Possible values: - **valid**: The validation was successful. - **invalid**: The validation failed. - **notValidated**: The validation was not performed because some services w'
  name: result
  type: string
- description: Type of check.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-validation-result-schema.json
slug: notification-webhooks-validation-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-validation-result-schema.json\",\n  \"title\": \"ValidationResult\",\n  \"description\": \"ValidationResult schema from Adyen API\",\n  \"properties\": {\n    \"result\": {\n      \"description\": \"The result of the check.\\n\\nPossible values:\\n\\n- **valid**: The validation was successful.\\n\\n- **invalid**: The validation failed.\\n\\n- **notValidated**: The validation was not performed because some services were unreachable or Adyen does not have the information needed to perform the check.\\n\\n- **notApplicable**: The validation is not applicable.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of check.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-validation-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ValidationResult
---
