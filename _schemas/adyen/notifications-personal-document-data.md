---
description: PersonalDocumentData schema from Adyen API
layout: schema
name: PersonalDocumentData
properties_list:
- description: The expiry date of the document, in ISO-8601 YYYY-MM-DD format. For example, **2000-01-31**.
  name: expirationDate
  type: string
- description: The country where the document was issued, in the two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) format. For example, **NL**.
  name: issuerCountry
  type: string
- description: The state where the document was issued (if applicable).
  name: issuerState
  type: string
- description: The number in the document.
  name: number
  type: string
- description: 'The type of the document. Possible values: **ID**, **DRIVINGLICENSE**, **PASSPORT**, **SOCIALSECURITY**, **VISA**. To delete an existing entry for a document `type`, send only the `type` field in your'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-personal-document-data-schema.json
slug: notifications-personal-document-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-personal-document-data-schema.json\",\n  \"title\": \"PersonalDocumentData\",\n  \"description\": \"PersonalDocumentData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expirationDate\": {\n      \"description\": \"The expiry date of the document, \\n in ISO-8601 YYYY-MM-DD format. For example, **2000-01-31**.\",\n      \"type\": \"string\"\n    },\n    \"issuerCountry\": {\n      \"description\": \"The country where the document was issued, in the two-character \\n[ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) format. For example, **NL**.\",\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"issuerState\": {\n      \"description\": \"The state where the document was issued (if applicable).\",\n      \"\
  type\": \"string\"\n    },\n    \"number\": {\n      \"description\": \"The number in the document.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of the document. Possible values: **ID**, **DRIVINGLICENSE**, **PASSPORT**, **SOCIALSECURITY**, **VISA**.\\n\\nTo delete an existing entry for a document `type`, send only the `type` field in your request. \",\n      \"enum\": [\n        \"DRIVINGLICENSE\",\n        \"ID\",\n        \"PASSPORT\",\n        \"SOCIALSECURITY\",\n        \"VISA\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-personal-document-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PersonalDocumentData
---
