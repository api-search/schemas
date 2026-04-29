---
description: Request body for emailing a price estimate to a customer
layout: schema
name: PriceEstimateEmailRequest
properties_list:
- description: Unique identifier of the price estimate to email
  name: estimate_id
  type: string
- description: Customer email address to send the estimate to
  name: customer_email
  type: string
- description: Customer full name for personalizing the email
  name: customer_name
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-price-estimate-email-request-schema.json
slug: api-connect-price-estimate-email-request
source_filename: api-connect-price-estimate-email-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-price-estimate-email-request-schema.json\",\n  \"title\": \"PriceEstimateEmailRequest\",\n  \"description\": \"Request body for emailing a price estimate to a customer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"estimate_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the price estimate to email\",\n      \"example\": \"est-500123\"\n    },\n    \"customer_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Customer email address to send the estimate to\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"customer_name\": {\n      \"type\": \"string\",\n      \"description\": \"Customer full name for personalizing the email\",\n      \"example\": \"Jane Smith\"\n    }\n  },\n  \"required\": [\n\
  \    \"estimate_id\",\n    \"customer_email\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-price-estimate-email-request-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: PriceEstimateEmailRequest
---
