---
description: ''
layout: schema
name: CustomField
properties_list:
- description: 'Custom field name like: `clientDateField1`, `clientDataField1`, `clientNumberField1`, `cardDateField1`, `cardDataField1`, `cardNumberField1`, `accountDateField1`, `accountDataField1`, `accountNumberFi'
  name: name
  type: string
- description: Custom field value. * In case of date value, it must be expressed in ISO 8601 format - YYYY-MM-DD. For example, 2022-01-16 * In case of data, it could be a free text that may contain alphanumeric lett
  name: value
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-custom-field-schema.json
slug: mastercard-card-issuance-custom-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CustomField\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Custom field name like: `clientDateField1`, `clientDataField1`, `clientNumberField1`, `cardDateField1`, `cardDataField1`, `cardNumberField1`, `accountDateField1`, `accountDataField1`, `accountNumberField1`. <BR/> Only 5 fields of each type are supported like clientDateField2, clientDateField3, clientDateField4, clientDateField5. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Custom field value.\\n* In case of date value, it must be expressed in ISO 8601 format - YYYY-MM-DD. For example, 2022-01-16\\n* In case of data, it could be a free text that may contain alphanumeric letters or special characters mentioned in the pattern field.\\\
  n* In case of number value, it is recommended to provide a number having maximum 12 digits before decimal and up to 5 digits after decimal. For example: 999999999999.99999\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-custom-field-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: CustomField
---
