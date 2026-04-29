---
description: Primary contact details of the merchant
layout: schema
name: PrimaryContact
properties_list:
- description: Job title of the primary contact
  name: jobTitle
  type: string
- description: First name of the primary contact
  name: firstName
  type: string
- description: Last name of the primary contact
  name: lastName
  type: string
- description: Phone number for primary contact
  name: phone
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-primary-contact-schema.json
slug: mastercard-ethoca-merchant-self-services-primary-contact
source_filename: mastercard-ethoca-merchant-self-services-primary-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PrimaryContact\",\n  \"type\": \"object\",\n  \"description\": \"Primary contact details of the merchant\",\n  \"properties\": {\n    \"jobTitle\": {\n      \"type\": \"string\",\n      \"description\": \"Job title of the primary contact\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the primary contact\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the primary contact\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number for primary contact\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-primary-contact-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: PrimaryContact
---
