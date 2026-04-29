---
description: Information about an Issuer as available on the server.
layout: schema
name: IssuerProfileDetails
properties_list:
- description: Unique Issuer identifier from the Mastercard Developers.
  name: clientId
  type: string
- description: Unique Issuer identifier assigned by Mastercard which remains the same across all Mastercard systems.
  name: customerId
  type: string
- description: Comma separated account range must be between 4 and 8 supported by an Issuer.
  name: supportedAccountRange
  type: string
- description: Status of an Issuer on the server. Possible values are Active and Suspended.
  name: status
  type: string
- description: Issuers email address
  name: email
  type: string
- description: DE 19 (Acquiring Institution Country Code) is the code of the country where the acquiring institution is located.
  name: countryCode
  type: string
- description: Privacy Notice URL.
  name: privacyNoticeURL
  type: string
- description: Terms and conditions URL for the given user.
  name: termsAndConditionURL
  type: string
- description: OPT out URL for the given user.
  name: optOutURL
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-carbon-calculator-experience-issuer-profile-details-schema.json
slug: mastercard-carbon-calculator-experience-issuer-profile-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IssuerProfileDetails\",\n  \"type\": \"object\",\n  \"description\": \"Information about an Issuer as available on the server.\",\n  \"properties\": {\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Issuer identifier from the Mastercard Developers.\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Issuer identifier assigned by Mastercard which remains the same across all Mastercard systems.\"\n    },\n    \"supportedAccountRange\": {\n      \"type\": \"string\",\n      \"description\": \"Comma separated account range must be between 4 and 8 supported by an Issuer.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of an Issuer on the server. Possible values are Active and Suspended.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Issuers email\
  \ address\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"DE 19 (Acquiring Institution Country Code) is the code of the country where the acquiring institution is located.\"\n    },\n    \"privacyNoticeURL\": {\n      \"type\": \"string\",\n      \"description\": \"Privacy Notice URL.\"\n    },\n    \"termsAndConditionURL\": {\n      \"type\": \"string\",\n      \"description\": \"Terms and conditions URL for the given user.\"\n    },\n    \"optOutURL\": {\n      \"type\": \"string\",\n      \"description\": \"OPT out URL for the given user.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-carbon-calculator-experience-issuer-profile-details-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: IssuerProfileDetails
---
