---
description: List of executives for the specified company identifier.
layout: schema
name: companyPeople
properties_list:
- description: FactSet Identifier for the company requested.
  name: fsymId
  type: string
- description: Email of the person
  name: email
  type: string
- description: FactSet Name of the person
  name: name
  type: string
- description: Job Function1
  name: jobFunction1
  type: string
- description: Job Function2
  name: jobFunction2
  type: string
- description: Job Function3
  name: jobFunction3
  type: string
- description: Job Function4
  name: jobFunction4
  type: string
- description: Main Phone Numbers of the executives.
  name: mainPhone
  type: string
- description: FactSet Entity Identifier for the Person.
  name: personId
  type: string
- description: Phone number of the executives.
  name: phone
  type: string
- description: Original identifier used for the request.
  name: requestId
  type: string
- description: Executive titles for a specified company.
  name: title
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-people-company-people-schema.json
slug: factset-people-company-people
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"companyPeople\",\n  \"type\": \"object\",\n  \"description\": \"List of executives for the specified company identifier.\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Identifier for the company requested.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email of the person\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Name of the person\"\n    },\n    \"jobFunction1\": {\n      \"type\": \"string\",\n      \"description\": \"Job Function1\"\n    },\n    \"jobFunction2\": {\n      \"type\": \"string\",\n      \"description\": \"Job Function2\"\n    },\n    \"jobFunction3\": {\n      \"type\": \"string\",\n      \"description\": \"Job Function3\"\n    },\n    \"jobFunction4\": {\n      \"type\": \"string\",\n      \"description\": \"Job Function4\"\n    },\n\
  \    \"mainPhone\": {\n      \"type\": \"string\",\n      \"description\": \"Main Phone Numbers of the executives.\"\n    },\n    \"personId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Entity Identifier for the Person.\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number of the executives.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Original identifier used for the request.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Executive titles for a specified company.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-people-company-people-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: companyPeople
---
