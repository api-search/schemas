---
description: UltimateParentCompany schema from Adyen API
layout: schema
name: UltimateParentCompany
properties_list:
- description: Address of the ultimate parent company.
  name: address
  type: object
- description: Details about the ultimate parent company's business.
  name: businessDetails
  type: object
- description: Adyen-generated unique alphanumeric identifier (UUID) for the entry, returned in the response when you create an ultimate parent company. Required when updating an existing entry in an `/updateAccount
  name: ultimateParentCompanyCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-ultimate-parent-company-schema.json
slug: notifications-ultimate-parent-company
source_filename: notifications-ultimate-parent-company-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-ultimate-parent-company-schema.json\",\n  \"title\": \"UltimateParentCompany\",\n  \"description\": \"UltimateParentCompany schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"Address of the ultimate parent company.\",\n      \"$ref\": \"#/components/schemas/ViasAddress\"\n    },\n    \"businessDetails\": {\n      \"description\": \"Details about the ultimate parent company's business.\",\n      \"$ref\": \"#/components/schemas/UltimateParentCompanyBusinessDetails\"\n    },\n    \"ultimateParentCompanyCode\": {\n      \"description\": \"Adyen-generated unique alphanumeric identifier (UUID) for the entry, returned in the response when you create an ultimate parent company. Required when updating an existing entry in an `/updateAccountHolder`\
  \ request.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-ultimate-parent-company-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UltimateParentCompany
---
