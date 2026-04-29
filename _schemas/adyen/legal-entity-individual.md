---
description: Individual schema from Adyen API
layout: schema
name: Individual
properties_list:
- description: The individual's birth information.
  name: birthData
  type: object
- description: The email address of the legal entity.
  name: email
  type: string
- description: Information about the individual's identification document.
  name: identificationData
  type: object
- description: The individual's name.
  name: name
  type: object
- description: The individual's nationality.
  name: nationality
  type: string
- description: The phone number of the legal entity.
  name: phone
  type: object
- description: The residential address of the individual.
  name: residentialAddress
  type: object
- description: The tax information of the individual.
  name: taxInformation
  type: array
- description: The website and app URL of the legal entity.
  name: webData
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-individual-schema.json
slug: legal-entity-individual
source_filename: legal-entity-individual-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-individual-schema.json\",\n  \"title\": \"Individual\",\n  \"description\": \"Individual schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"birthData\": {\n      \"description\": \"The individual's birth information.\",\n      \"$ref\": \"#/components/schemas/BirthData\"\n    },\n    \"email\": {\n      \"description\": \"The email address of the legal entity.\",\n      \"type\": \"string\"\n    },\n    \"identificationData\": {\n      \"description\": \"Information about the individual's identification document.\",\n      \"$ref\": \"#/components/schemas/IdentificationData\"\n    },\n    \"name\": {\n      \"description\": \"The individual's name.\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"nationality\": {\n      \"description\": \"The individual's nationality.\"\
  ,\n      \"type\": \"string\"\n    },\n    \"phone\": {\n      \"description\": \"The phone number of the legal entity.\",\n      \"$ref\": \"#/components/schemas/PhoneNumber\"\n    },\n    \"residentialAddress\": {\n      \"description\": \"The residential address of the individual.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"taxInformation\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The tax information of the individual.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaxInformation\"\n      },\n      \"type\": \"array\"\n    },\n    \"webData\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"1\",\n      \"description\": \"The website and app URL of the legal entity.\",\n      \"$ref\": \"#/components/schemas/WebData\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"residentialAddress\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-individual-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Individual
---
