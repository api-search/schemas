---
description: Travel Information, Applicable only if the client has a prepaid card.
layout: schema
name: TravelDetails
properties_list:
- description: Indicates the purpose of travel for which the client will be using the card. For example, medical reasons, cultural trip, and business trip and so on. <BR/> Valid values are as configured on portal in
  name: type
  type: string
- description: Start date of the planned travel. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required if travel type is provided. <br/> Format - It is expressed in ISO 8601 - `YYYY-MM-DD`
  name: startDate
  type: string
- description: End date of the planned travel. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required if travel type is provided. <br/> Format - It is expressed in ISO 8601 - `YYYY-MM-DD`
  name: endDate
  type: string
- description: Country Code where client is traveling to. <BR/> Expressed as a 2-letter (Alpha-2) country code as defined in ISO 3166. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required if t
  name: country
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-travel-details-schema.json
slug: mastercard-card-issuance-travel-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TravelDetails\",\n  \"type\": \"object\",\n  \"description\": \"Travel Information, Applicable only if the client has a prepaid card.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the purpose of travel for which the client will be using the card. For example, medical reasons, cultural trip, and business trip and so on. <BR/> Valid values are as configured on portal in Card Management > Program Setup >Travel Type Configuration section. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"Start date of the planned travel. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required if travel type is provided. <br/> Format - It is expressed in ISO 8601 - `YYYY-MM-DD`\"\n    },\n    \"endDate\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"End date of the planned travel. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required if travel type is provided. <br/> Format - It is expressed in ISO 8601 - `YYYY-MM-DD`\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country Code where client is traveling to. <BR/> Expressed as a 2-letter (Alpha-2) country code as defined in ISO 3166. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required if travel type is provided.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-travel-details-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: TravelDetails
---
