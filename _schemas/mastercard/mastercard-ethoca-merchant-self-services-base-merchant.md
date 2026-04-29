---
description: Base merchant model schema
layout: schema
name: BaseMerchant
properties_list:
- description: Name of the merchant that the item was purchased from.
  name: name
  type: string
- description: A four-digit number listed in ISO 18245 for retail financial services. MCC is used to classify the business by the type of goods or services it provides.
  name: categoryCode
  type: string
- description: The earliest date an Issuer can search for orders (i.e. the date an Issuer cannot search before). Date-Time must be in [ISO 8601 format](https://datatracker.ietf.org/doc/html/rfc3339#section-5.6)
  name: orderAvailabilityDateTime
  type: string
- description: The number of months worth of data you have made available to search on.
  name: orderHistoryMonths
  type: integer
- description: The numbers of days that need to elapse between an authorization for a purchase and when the purchase can be searched on.
  name: orderLatencyDays
  type: integer
- description: Industry Code is used to classify the business by the type of industry.
  name: industryCode
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-base-merchant-schema.json
slug: mastercard-ethoca-merchant-self-services-base-merchant
source_filename: mastercard-ethoca-merchant-self-services-base-merchant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BaseMerchant\",\n  \"type\": \"object\",\n  \"description\": \"Base merchant model schema\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the merchant that the item was purchased from.\"\n    },\n    \"categoryCode\": {\n      \"type\": \"string\",\n      \"description\": \"A four-digit number listed in ISO 18245 for retail financial services. MCC is used to classify the business by the type of goods or services it provides.\"\n    },\n    \"orderAvailabilityDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The earliest date an Issuer can search for orders (i.e. the date an Issuer cannot search before). Date-Time must be in [ISO 8601 format](https://datatracker.ietf.org/doc/html/rfc3339#section-5.6)\"\n    },\n    \"orderHistoryMonths\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of months worth\
  \ of data you have made available to search on.\"\n    },\n    \"orderLatencyDays\": {\n      \"type\": \"integer\",\n      \"description\": \"The numbers of days that need to elapse between an authorization for a purchase and when the purchase can be searched on. \"\n    },\n    \"industryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Industry Code is used to classify the business by the type of industry.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-base-merchant-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: BaseMerchant
---
