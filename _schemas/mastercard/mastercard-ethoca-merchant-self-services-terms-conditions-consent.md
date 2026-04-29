---
description: ''
layout: schema
name: TermsConditionsConsent
properties_list:
- description: Date stamp in which the sub-merchant provided his consent on the terms and conditions. Date must be in [ISO 8601 format](https://datatracker.ietf.org/doc/html/rfc3339#section-5.6)
  name: date
  type: string
- description: First name of person that gave consent
  name: firstName
  type: string
- description: Last name of person that gave consent
  name: lastName
  type: string
- description: Job title of person that gave consent
  name: jobTitle
  type: string
- description: Universally Unique Identifier (UUID) of the consent that the user consented to
  name: consentUuid
  type: string
- description: Version of the consent that the user consented to
  name: consentVersion
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-terms-conditions-consent-schema.json
slug: mastercard-ethoca-merchant-self-services-terms-conditions-consent
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TermsConditionsConsent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Date stamp in which the sub-merchant provided his consent on the terms and conditions. Date must be in [ISO 8601 format](https://datatracker.ietf.org/doc/html/rfc3339#section-5.6)\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name of person that gave consent\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of person that gave consent\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\",\n      \"description\": \"Job title of person that gave consent\"\n    },\n    \"consentUuid\": {\n      \"type\": \"string\",\n      \"description\": \"Universally Unique Identifier (UUID) of the consent that the user consented to\"\n    },\n    \"consentVersion\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Version of the consent that the user consented to\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-terms-conditions-consent-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: TermsConditionsConsent
---
