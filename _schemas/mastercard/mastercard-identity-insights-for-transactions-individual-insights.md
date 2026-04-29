---
description: The details associated with the individual insights.
layout: schema
name: IndividualInsights
properties_list:
- description: ''
  name: alerts
  type: array
- description: An array containing warning messages.
  name: warnings
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-individual-insights-schema.json
slug: mastercard-identity-insights-for-transactions-individual-insights
source_filename: mastercard-identity-insights-for-transactions-individual-insights-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IndividualInsights\",\n  \"type\": \"object\",\n  \"description\": \"The details associated with the individual insights.\",\n  \"properties\": {\n    \"alerts\": {\n      \"type\": \"array\"\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"description\": \"An array containing warning messages.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-individual-insights-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: IndividualInsights
---
