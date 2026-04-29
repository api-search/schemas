---
description: It contains the identifications of the stored value account or the stored value card, and the associated product sold by the Sale System for stored value requests. Identification of the stored value account or the stored value card.
layout: schema
name: StoredValueAccountID
properties_list:
- description: ''
  name: StoredValueAccountType
  type: object
- description: ''
  name: StoredValueProvider
  type: string
- description: ''
  name: OwnerName
  type: string
- description: ''
  name: ExpiryDate
  type: integer
- description: ''
  name: EntryMode
  type: object
- description: ''
  name: IdentificationType
  type: object
- description: ''
  name: StoredValueID
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-stored-value-account-id-schema.json
slug: terminal-stored-value-account-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-stored-value-account-id-schema.json\",\n  \"title\": \"StoredValueAccountID\",\n  \"description\": \"It contains the identifications of the stored value account or the stored value card, and the associated product sold by the Sale System for stored value requests. Identification of the stored value account or the stored value card.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StoredValueAccountType\": {\n      \"$ref\": \"#/components/schemas/StoredValueAccountType\"\n    },\n    \"StoredValueProvider\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"OwnerName\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"ExpiryDate\": {\n      \"type\": \"integer\",\n      \"minimum\": 4,\n      \"maximum\": 4\n    },\n    \"EntryMode\": {\n      \"\
  $ref\": \"#/components/schemas/EntryMode\"\n    },\n    \"IdentificationType\": {\n      \"$ref\": \"#/components/schemas/IdentificationType\"\n    },\n    \"StoredValueID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    }\n  },\n  \"required\": [\n    \"StoredValueAccountType\",\n    \"EntryMode\",\n    \"IdentificationType\",\n    \"StoredValueID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-stored-value-account-id-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredValueAccountID
---
